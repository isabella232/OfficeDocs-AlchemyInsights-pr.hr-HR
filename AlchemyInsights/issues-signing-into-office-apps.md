---
title: Potpisivanje Office apps problemi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938160"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Popravljanje Office apps "Trusted Platform module vaše računalo ne radi ispravno" poruka

Da biste ispravili tu pogrešku, pokušajte sljedeće:

- Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Očisti Office vjerodajnice](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću Windows upravitelj vjerodajnica.<br/>
    **Napomena:** Putova registra za Office 2016 ste promijenili 16.0. (Prije: \Software\Microsoft\Office\16.0\Common\Identity\)
- Pokušajte [postupka oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) da biste ispravili pogreške Trusted Platform Module (TPM).
- Postaviti na EnableADAL = 0 pomoću sljedećih koraka:  
    1. Desnom tipkom miša pritisnite gumb Start sustava Windows, odaberite **Pokreni**, upišite **regedit**i odaberite **u redu**.
    2. Za odaberite **da** Dopusti uređivač registra da biste napravili promjene na uređaj.
    3. U programu Registry Editor dodajte DWORD vrijednost **EnableADAL** s postavkom **0** pod HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Za dodatne informacije pogledajte [veze problemi u prijavu nakon ažuriranja za Office 2016 build 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).