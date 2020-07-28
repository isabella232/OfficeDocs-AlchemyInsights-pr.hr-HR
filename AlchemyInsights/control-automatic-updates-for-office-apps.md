---
title: Upravljanje automatskim ažuriranjima za aplikacije sustava Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438838"
---
# <a name="control-automatic-updates-for-office-apps"></a>Upravljanje automatskim ažuriranjima za aplikacije sustava Office

Ažuriranja za aplikacije sustava Office prema zadanim se postavkama automatski preuzimaju i primjenjuju u pozadini bez intervencije korisnika. Međutim, administratori mogu kontrolirati kako se ažuriranja primjenjuju pomoću postavki servisa Office Update. Postavke ažuriranja administratorima omogućuju omogućivanje ili onemogućivanje automatskog ažuriranja, prikaz ili skrivanje gumba **Ažuriraj sada** u sustavu Office, postavite rokove ažuriranja i još mnogo toga. Detaljne informacije potražite u članku:

- [Konfiguriranje postavki ažuriranja za Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatsko ažuriranje za Office nije omogućeno](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definiranje načina ažuriranja sustava Office nakon instalacije](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Da biste pregledali postojeće postavke ažuriranja primijenjene na klijentsko računalo, slijedite ove korake:

1. OpenBSD Registry Editor odlaskom na **Početak**  >  **Trčanje**  >  **regentstvo.**
2. Prijeđite na sljedeće mjesto i pregledajte postavke ažuriranja sustava Office:  
    A. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    B. ClickToRun\Konfiguracija

**Napomena:**  Ako je postavljen ključ OfficeMgmtCOM, **možda**će vam se prikazati poruka "Ažuriranjima upravlja administrator sustava" u  >  **Account**  >  **ažuriranjima sustava Office**Account Office . Dodatne informacije [potražite u odjeljku Upravljanje ažuriranjima aplikacija microsoft 365 s programom Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  