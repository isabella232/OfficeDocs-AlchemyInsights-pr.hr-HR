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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938158"
---
# <a name="issues-signing-in-to-office-apps"></a>Potpisivanje Office apps problemi

Da biste riješili probleme za prijavu s Office apps, pokušajte sljedeće:

- Uklonite sve račune rad, osim zahvaćeni račun pomoću Windows postavke > **pristup poslu ili u školi**.
- [Očisti Office vjerodajnice](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću Windows upravitelj vjerodajnica.<br/>
    **Napomena:** Putova registra za Office 2016 ste promijenili 16.0. (Prije: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otvorite Office app, odaberite **datoteku** > **račun** > **Odjava**. Zatim prijavite putem korisničkog računa s valjanu licencu. Za detaljnije informacije pogledajte [račune u Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Za Mac, vidjeti [ne mogu prijaviti u 2016 Office za Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Ako dođe do pogreške pri povezivanju s Office 365 pomoću Office 2013, omogućiti Moderna provjeru autentičnosti klijenta sustava Office.

Dodatne informacije potražite u sljedećem članku:
- [Ne možete se prijaviti na Office 365, Azure ili Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Povezivanjem u prijavu nakon ažuriranja za Office 2016 build 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Nažalost, drugi račun iz vaše organizacije već prijavljeni na ovom računalu" u Officeu](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Rješavanje problema u znak s Office Moderna provjere autentičnosti kada koristite ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)