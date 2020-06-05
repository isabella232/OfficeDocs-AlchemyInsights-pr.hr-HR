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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579929"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Ispravak poruke aplikacije sustava Microsoft 365 "Nažalost, već je prijavljen drugi račun iz tvrtke ili ustanove"

Da biste ispravili tu pogrešku, pokušajte sljedeće:

- Uklonite sve poslovne račune, osim zahvaćenog računa, pomoću postavki sustava Windows > **Access posao ili školu**.
- [Izbrišite vjerodajnice sustava Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica sustava Windows.<br/>
    **Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0. (Npr.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otvorite aplikaciju **File**sustava Office, odaberite  >  Odjava**računa**  >  **datoteke**. Zatim se prijavite pomoću korisničkog računa s valjanom licencom. Detaljne informacije potražite u članku [Računi u sustavu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Za Mac pročitajte [Nije moguća prijava u aplikaciju sustava Office 2016 za Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Dodatne informacije potražite [u odjeljku "Nažalost, na ovom je računalu već prijavljen drugi račun tvrtke ili ustanove" u sustavu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).