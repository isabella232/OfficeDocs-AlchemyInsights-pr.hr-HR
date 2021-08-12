---
title: Upravljanje automatskim ažuriranjima za Office aplikacije
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: f162f11f678e8673d85e52cd9e54cedd7bd6e6a3aee87fcb2731a06d2698ea6a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929873"
---
# <a name="control-automatic-updates-for-office-apps"></a>Upravljanje automatskim ažuriranjima za Office aplikacije

Ažuriranja za aplikacije Office po zadanom se preuzimaju automatski i primjenjuju u pozadini bez intervencije korisnika. No administratori mogu kontrolirati kako se ažuriranja primjenjuju pomoću postavki Office ažuriranje. Postavke ažuriranja administratorima omogućuju omogućivanje ili onemogućivanje  automatskih ažuriranja, prikaz ili skrivanje gumba Ažuriraj odmah u Office, postavljanje rokova za ažuriranje i još mnogo toga. Detaljne informacije potražite u članku:

- [Konfiguriranje postavki ažuriranja za Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatsko ažuriranje za Office nije omogućeno](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definiranje Office ažuriranja nakon instalacije](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Da biste pregledali postojeće postavke ažuriranja primijenjene na klijentsko računalo, slijedite ove korake:

1. Otvorite uređivač registra tako da otvorite **Pokreni**  >    >  **regedit**.
2. Prijeđite na sljedeće mjesto i pregledajte postavke Office Ažuriranje:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Napomena**  Ako je postavljen ključ OfficeMgmtCOM, možda ćete vidjeti poruku "Ažuriranja upravlja administrator sustava" u odjeljku **Office**  >  **Račun**  >  **Office ažuriranja**. Dodatne informacije potražite u članku [Upravljanje ažuriranjima za Microsoft 365 Apps s Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  