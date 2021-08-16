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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028032"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Rješavanje problema Microsoft 365 "Nažalost, već je prijavljen drugi račun tvrtke ili ustanove".

Da biste ispravili tu pogrešku, pokušajte sljedeće:

- Uklonite sve poslovne račune, osim zahvaćenog računa, pomoću Windows Postavke > **accessa ili škole.**
- [Poništite Office pomoću](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) upravitelja Windows vjerodajnica.<br/>
    **Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otvorite aplikacija Office, odaberite   >    >  **Odjava s računa datoteke**. Zatim se prijavite pomoću korisničkog računa s valjanom licencom. Detaljne informacije potražite u članku [Računi u sustavu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Za Mac pročitajte [Nije moguća prijava u aplikaciju sustava Office 2016 za Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Dodatne informacije potražite u članku "Nažalost, drugi je račun tvrtke ili ustanove već prijavljen na [ovom računalu" u Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).