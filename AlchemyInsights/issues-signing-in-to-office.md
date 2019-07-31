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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938159"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Prazan prijavu zaslon u Office apps

Da biste riješili taj problem, pokušajte sljedeće:
- Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Vrati mogućnosti programa Internet Explorer: idite na **Alati** > **Internet opcije** > **Napredno** > **Vraćanje postavki programa Internet Explorer** (Napomena će izgubiti prilagođene postavke), a zatim pokušajte ponovno potpisivanja Office.
- Onemogući Windows Defender aplikacije Guard (WDAG) ili bilo koji sličan vatrozid ili protuvirusni program:
    1. Na upravljačkoj ploči, idite na **programe**i odabrati **značajke Windows uključivanje ili isključivanje**.
    2. Ako je omogućen Guard aplikacije Windows Defender, pokušajte ga onemogućiti.<br/>
    **Napomena:** Možda ćete morati ponovo pokrenuti računalo.
- Osigurajte da Microsoft.AAD.BrokerPlugin [AAD WAM dodatak](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne blokira aplikacije ili vatrozida/funkcijama za zaštitu-virus program.
- [Očisti Office vjerodajnice](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću Windows upravitelj vjerodajnica.<br/>
    **Napomena:** Putova registra za Office 2016 ste promijenili 16.0. (Prije: \Software\Microsoft\Office\16.0\Common\Identity\)

Za dodatne informacije pogledajte [veze problemi u prijavu nakon ažuriranja za Office 2016 build 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).