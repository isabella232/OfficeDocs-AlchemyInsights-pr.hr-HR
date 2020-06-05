---
title: Problemi s prijavom u aplikacije sustava Microsoft 365
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
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579893"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazan zaslon za prijavu u aplikacijama Microsoft 365

Da biste riješili taj problem, pokušajte sljedeće:
- Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Vraćanje izvornih mogućnosti preglednika Internet Explorer: idite na **Alati**  >  **Internetske mogućnosti**  >  **Advanced**  >  **Napredne postavke preglednika Internet Explorer** (imajte na umu da ćete izgubiti prilagođene postavke), a zatim se ponovno pokušajte prijaviti u Office.
- Onesposobiti Windows Branitelj Aplikacija Čuvati (WDAG) ili bilo koji sličan firewall ili protu-- virus plan:
    1. Na upravljačkoj ploči idite na **Programi**, a zatim uključite **ili isključite značajke sustava Windows**.
    2. Ako je windows defender application guard omogućen, pokušajte ga onemogućiti.<br/>
    **Napomena:** Možda ćete morati ponovo pokrenuti računalo.
- Provjerite da dodatak Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne blokira nijedan program za aplikaciju ili vatrozid/protuvirusni program.
- [Izbrišite vjerodajnice sustava Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica sustava Windows.<br/>
    **Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0. (Npr.: \Software\Microsoft\Office\16.0\Common\Identity\)

Dodatne informacije [potražite u odjeljku Problemi s povezivanjem prilikom ažuriranja na međuverziju sustava Office 2016 16.0.7967 u sustavu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).