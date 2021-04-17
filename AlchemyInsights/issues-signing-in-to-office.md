---
title: Problemi prilikom prijave u aplikacije sustava Microsoft 365
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
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833023"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazan zaslon za prijavu u aplikacije Microsoft 365

Da biste riješili taj problem, pokušajte sljedeće:
- Instalirajte najnovija ažuriranja za [Windows i](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Ponovno postavite mogućnosti preglednika Internet Explorer: otvorite Alati za internetske mogućnosti Napredno ponovno postavljanje postavki preglednika Internet Explorer (imajte na umu da ćete izgubiti prilagođene postavke), a  >    >    >   zatim se ponovno pokušajte prijaviti u Office.
- Onemogućite Windows Defender Application Guard (WDAG) ili bilo koji sličan vatrozid ili antivirusni program:
    1. Na upravljačkoj ploči idite **na Programi**, a zatim **odaberite Uključi ili isključi značajke sustava Windows**.
    2. Ako je omogućen Windows Defender Application Guard, pokušajte ga onemogućiti.<br/>
    **Napomena:** Možda ćete morati ponovno pokrenuti računalo.
- Provjerite ne blokira li programski dodatak Microsoft.AAD.BrokerPlugin [AAD WAM.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)
- [Poništite vjerodajnice sustava Office pomoću](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) upravitelja vjerodajnica sustava Windows.<br/>
    **Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Dodatne informacije potražite u članku Problemi s povezivanjem prilikom prijave nakon ažuriranja na međuverziju [16.0.7967 sustava Office 2016 u sustavu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).