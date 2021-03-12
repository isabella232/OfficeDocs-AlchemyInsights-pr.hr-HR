---
title: Postavljanje značajke ClientAccessServerEnabled u True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743771"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Postavljanje značajke ClientAccessServerEnabled u True

Ako ne možete otvoriti šifriranu poruku e-pošte i umjesto njega vidjeti privitak s **rpmsg** -a, slijedite sljedeće korake:

1. Spojite se na PowerShell sustava Exchange Online.

> [!NOTE]
> Da biste se povezali sa komponenti Exchange Online PowerShell, morate se prijaviti pomoću globalnog administratora ili administratora za administratore sustava Exchange.

   je. Otvorite Windows PowerShell, a zatim pokrenite sljedeću naredbu: `$UserCredential = Get-Credential`
b. U dijaloškom okviru **zahtjev za vjerodajnice vjerodajnica za Windows PowerShell** unesite svoj račun za rad ili školovanje i lozinku, c. Kliknite **U redu**. 

2. Pokrenite sljedeću naredbu da biste stvorili novu sesiju:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    je. Izvršite sljedeću naredbu:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Pokreni `Get-IRMConfiguration` naredbu.

4. Provjerite postavku **Clientaccessserverenabled** . 

    je. Ako je postavka **Clientaccessserverenabled** postavljena na **False**, pokrenite sljedeći cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Uvijek zatvarate sesiju PowerShell uz sljedeću naredbu: `Remove-PSSession $Session`

Dodatne informacije potražite u članku [Microsoft Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

