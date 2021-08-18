---
title: Problemi prilikom prijave u Microsoft 365 aplikacije
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088028"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazan zaslon za prijavu u Microsoft 365 aplikacijama

Da biste riješili taj problem, pokušajte sljedeće:
- Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [i Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Ponovno postavite mogućnosti preglednika Internet Explorer: idite na Alati Internet  >    >    >  **Options Advanced Reset Internet Explorer Postavke** (imajte na umu da ćete izgubiti prilagođene postavke), a zatim se ponovno Office prijaviti.
- Onemogućivanje Windows Defender Application Guard (WDAG) ili bilo kojeg sličnog vatrozida ili antivirusnog programa:
    1. Na upravljačkoj ploči idite **na Programi**, a zatim **odaberite Uključi Windows ili isključi** značajke .
    2. Ako Windows Defender Application Guard omogućen, pokušajte ga onemogućiti.<br/>
    **Napomena:** Možda ćete morati ponovno pokrenuti računalo.
- Provjerite ne blokira li programski dodatak Microsoft.AAD.BrokerPlugin [AAD WAM.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)
- [Poništite Office pomoću](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) upravitelja Windows vjerodajnica.<br/>
    **Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Dodatne informacije potražite u članku Problemi s povezivanjem prilikom prijave nakon ažuriranja [za Office 2016 međuverziju 16.0.7967 na servisu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).