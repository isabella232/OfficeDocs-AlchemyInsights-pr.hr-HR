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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695315"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Popravljanje aplikacija Microsoft 365 "Žao nam je, još jedan račun iz vaše tvrtke ili ustanove već je potpisan u" poruci

Da biste ispravili tu pogrešku, pokušajte sljedeće:

- Uklonite sve radne račune, osim izvještačenog računa, pomoću postavki sustava Windows > **pristupu radu ili školi**.
- [Poništite vjerodajnice sustava Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica za Windows.<br/>
    **Upozorenje:** Putevi registra za Office 2016 promijenili su se u 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otvorite aplikaciju sustava Office, odaberite odjavu računa za **datoteke**  >  **Account**  >  **Sign Out**. Zatim se prijavite pomoću korisničkog računa s valjanom licencom. Detaljne informacije potražite u članku [Računi u sustavu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Za Mac pročitajte [Nije moguća prijava u aplikaciju sustava Office 2016 za Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Dodatne informacije potražite u članku ["Žao nam je, još jedan račun iz vaše tvrtke ili ustanove već je prijavljen na ovom računalu" u sustavu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).