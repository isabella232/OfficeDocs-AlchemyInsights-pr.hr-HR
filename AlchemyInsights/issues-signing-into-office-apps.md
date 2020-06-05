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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579857"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Ispravljanje poruke aplikacije Microsoft 365 "Modul pouzdane platforme vašeg računala ne funkcionira ispravno"

Da biste ispravili tu pogrešku, pokušajte sljedeće:

- Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Izbrišite vjerodajnice sustava Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica sustava Windows.<br/>
    **Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0. (Npr.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Isprobajte [postupak oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) da biste ispravili pogreške trusted platform module (TPM).
- Postavite EnableADAL = 0 pomoću sljedećih koraka:  
    1. Desnom tipkom miša kliknite gumb Start sustava Windows, odaberite **Pokreni**, upišite **regedit**, a zatim odaberite **U redu**.
    2. Odaberite **Da** da biste uređivaču registra omogućili izmjene uređaja.
    3. In Registry Editor, dodati DWORD vrijednost od **EnableADAL** sa postavljanje od **0** pod HKEY_CURRENT_USER\SoftwareMicrosoft\Office16.0\Common\Identity.

Dodatne informacije [potražite u odjeljku Problemi s povezivanjem prilikom ažuriranja na međuverziju sustava Office 2016 16.0.7967 u sustavu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).