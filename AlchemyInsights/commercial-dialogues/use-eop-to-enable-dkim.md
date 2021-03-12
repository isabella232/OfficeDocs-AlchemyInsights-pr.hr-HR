---
title: Omogućivanje servisa DEKIM za određenu domenu pomoću komponente Exchange Online PowerShell
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743732"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Omogućivanje servisa DEKIM za određenu domenu pomoću komponente Exchange Online PowerShell

Ako u centru za administratore ne možete stvoriti DNS zapise servisa d-a, pokušajte koristiti PowerShell sustava Exchange Online. 

Da biste stvorili DNS zapis u programu Microsoft Exchange Online, slijedite sljedeće korake:

1. Otvorite Windows PowerShell kao administrator, a zatim u opisnim redoslijedom pokrenite sljedeće naredbe:

    je. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Ako imate problema s povezivanjem sa komponenti Exchange Online PowerShell, pročitajte članak [Povezivanje s PowerShell sustava Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Kada se povežete sa sustavom Exchange Online PowerShell, pokrenite sljedeću naredbu:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Kada se gornja naredba uspješno izvrši, pokrenite sljedeću naredbu da biste prekinuli sesiju PowerShell sustava Exchange Online:

    `Remove-PSSession $Session` 



