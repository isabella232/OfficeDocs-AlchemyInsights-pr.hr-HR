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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832995"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Popravljanje aplikacije Microsoft 365 "Modul pouzdane platforme na računalu ne funkcionira pravilno"

Da biste ispravili tu pogrešku, pokušajte sljedeće:

- Instalirajte najnovija ažuriranja za [Windows i](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Poništite vjerodajnice sustava Office pomoću](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) upravitelja vjerodajnica sustava Windows.<br/>
    **Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Isprobajte [postupak oporavka korisnika da](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) biste riješili pogreške modula pouzdane platforme (TPM).
- Postavite EnableADAL = 0 pomoću sljedećih koraka:  
    1. Desnom tipkom miša kliknite gumb Start sustava Windows, odaberite **Pokreni**, upišite **regedit**, a zatim odaberite U **redu**.
    2. Odaberite **Da** da biste uređivaču registra omogućili unos promjena na uređaj.
    3. U uređivaču registra dodajte DWORD vrijednost **EnableADAL** s postavkom **0 u** odjeljku HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Dodatne informacije potražite u članku Problemi s povezivanjem prilikom prijave nakon ažuriranja na međuverziju [16.0.7967 sustava Office 2016 u sustavu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).