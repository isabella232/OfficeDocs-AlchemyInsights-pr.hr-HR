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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986883"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Popravljanje Microsoft 365 aplikacije "Modul pouzdane platforme na računalu ne funkcionira pravilno"

Da biste ispravili tu pogrešku, pokušajte sljedeće:

- Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [i Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Poništite Office pomoću](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) upravitelja Windows vjerodajnica.<br/>
    **Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Isprobajte [postupak oporavka korisnika da](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) biste riješili pogreške modula pouzdane platforme (TPM).
- Postavite EnableADAL = 0 pomoću sljedećih koraka:  
    1. Desnom tipkom miša kliknite gumb Windows Start, odaberite **Pokreni**, upišite **regedit**, a zatim odaberite U **redu**.
    2. Odaberite **Da** da biste uređivaču registra omogućili unos promjena na uređaj.
    3. U uređivaču registra dodajte DWORD vrijednost **EnableADAL** s postavkom **0 u** odjeljku HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Dodatne informacije potražite u članku Problemi s povezivanjem prilikom prijave nakon ažuriranja [za Office 2016 međuverziju 16.0.7967 na servisu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).