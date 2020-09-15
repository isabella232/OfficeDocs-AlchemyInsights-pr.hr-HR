---
title: Problemi s prijavom u aplikacije Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695279"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazni zaslon za prijavu u aplikacijama Microsoft 365

Da biste riješili taj problem, pokušajte sljedeće:
- Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Ponovno postavljanje mogućnosti u pregledniku Internet Explorer: Idite na **Alati**za  >  **napredne internetske mogućnosti**  >  **Advanced**  >  **ponovno postavljanje postavki preglednika Internet Explorer** (primijetite da ćete izgubiti prilagođene postavke), a zatim se pokušajte ponovno prijaviti u Office.
- Onemogućite čuvar aplikacije programa Windows Defender (WDAG) ili bilo koji sličan vatrozid ili protuvirusni program:
    1. Na upravljačkoj ploči otvorite **program**, a zatim odaberite **Uključivanje i isključivanje značajki sustava Windows**.
    2. Ako je omogućen čuvar aplikacije programa Windows Defender, pokušajte ga onemogućiti.<br/>
    **Upozorenje:** Možda ćete morati ponovno pokrenuti računalo.
- Provjerite nije li dodatak Microsoft. AAD. [brokerskog dodatka AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nije blokiran bilo kojim aplikacijom ili vatrozidom/antivirusni programom.
- [Poništite vjerodajnice sustava Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica za Windows.<br/>
    **Upozorenje:** Putevi registra za Office 2016 promijenili su se u 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Dodatne informacije potražite u članku [Problemi s povezivanjem u programu za prijavu nakon ažuriranja na Office 2016 međuverzija 16.0.7967 u sustavu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).