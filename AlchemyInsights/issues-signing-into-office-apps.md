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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695171"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Ispravljanje aplikacija Microsoft 365 "Trusted Platform modul za vaše računalo ne funkcionira pravilno" poruka

Da biste ispravili tu pogrešku, pokušajte sljedeće:

- Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Poništite vjerodajnice sustava Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica za Windows.<br/>
    **Upozorenje:** Putevi registra za Office 2016 promijenili su se u 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Isprobajte [postupak oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) da biste riješili pogreške pouzdanih Platform MODULE (TPM-a).
- Postavite EnableADAL = 0 pomoću sljedećih koraka:  
    1. Desnom tipkom miša kliknite gumb Start sustava Windows, odaberite **Pokreni**, upišite **regedit**, a zatim odaberite **u redu**.
    2. Odaberite **da** da bi uređivač registra omogućio promjene na uređaju.
    3. U uređivaču registra dodajte vrijednost DWORD za **Enableadal** s postavkom **0** u odjeljku HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.

Dodatne informacije potražite u članku [Problemi s povezivanjem u programu za prijavu nakon ažuriranja na Office 2016 međuverzija 16.0.7967 u sustavu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).