---
title: Postavljanje clientaccessserverEnabled na True
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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994857"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Postavljanje clientaccessserverEnabled na True

Ako ne možete otvoriti šifriranu poruku e-pošte i umjesto toga vidjeti **privitak rpmsg,** učinite sljedeće:

1. Povezivanje na Exchange Online PowerShell.

> [!NOTE]
> Da biste se Exchange Online s ljuskom PowerShell, morate se prijaviti pomoću globalnog administratora ili Exchange administratorskog računa.

   a. Otvorite Windows PowerShell, a zatim pokrenite sljedeću naredbu:`$UserCredential = Get-Credential`
b. U **dijaloškom Windows PowerShell zahtjev za** vjerodajnice unesite račun i lozinku za posao ili školu, c. Kliknite **U redu**. 

2. Pokrenite sljedeću naredbu da biste stvorili novu sesiju:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Izvršite sljedeću naredbu:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Pokreni `Get-IRMConfiguration` naredbu.

4. Provjerite **postavku ClientAccessServerEnabled.** 

    a. Ako **je postavka ClientAccessServerEnabled** postavljena na **False**, pokrenite sljedeći cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Sesiju ljuske powershell uvijek zatvorite sljedećom naredbom: `Remove-PSSession $Session`

Dodatne informacije potražite u članku [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

