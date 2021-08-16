---
title: Omogućivanje Exchange Online komponente PowerShell za određenu domenu pomoću komponente PowerShell
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070284"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Omogućivanje Exchange Online komponente PowerShell za određenu domenu pomoću komponente PowerShell

Ako U centru za administratore ne možete stvoriti DKIM DNS zapise, pokušajte koristiti Exchange Online PowerShell. 

Da biste Stvorili DKIM DNS zapis pomoću komponente Exchange Online PowerShell, učinite sljedeće:

1. Otvorite Windows PowerShell kao administrator i pokrenite sljedeće naredbe u opisanom slijedu:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Ako imate problema s povezivanjem Exchange Online ljuske PowerShell, [pogledajte Povezivanje na Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Kada se povežete s Exchange Online PowerShell, pokrenite sljedeću naredbu:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Kada se navedena naredba uspješno izvrši, pokrenite sljedeću naredbu da biste prekinuli sesiju Exchange Online PowerShell:

    `Remove-PSSession $Session` 



