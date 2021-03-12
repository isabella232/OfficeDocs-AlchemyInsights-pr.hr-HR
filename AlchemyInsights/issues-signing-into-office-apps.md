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
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709098"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Ispravljanje aplikacija Microsoft 365 "Trusted Platform modul za vaše računalo ne funkcionira pravilno" poruka

Da biste ispravili tu pogrešku, pokušajte sljedeće:

- Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Poništite vjerodajnice sustava Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica za Windows.<br/>
    **Upozorenje:** Putevi registra za Office 2016 promijenili su se u 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Isprobajte [postupak oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) da biste riješili pogreške pouzdanih Platform MODULE (TPM-a).
- Postavite EnableADAL = 0 pomoću sljedećih koraka:  
    1. Desnom tipkom miša kliknite gumb Start sustava Windows, odaberite **Pokreni**, upišite **regedit**, a zatim odaberite **u redu**.
    2. Odaberite **da** da bi uređivač registra omogućio promjene na uređaju.
    3. U uređivaču registra dodajte vrijednost DWORD za **Enableadal** s postavkom **0** u odjeljku HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Dodatne informacije potražite u članku [Problemi s povezivanjem u programu za prijavu nakon ažuriranja na Office 2016 međuverzija 16.0.7967 u sustavu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).