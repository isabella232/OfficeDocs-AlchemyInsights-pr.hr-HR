---
title: Kontrola automatskih ažuriranja za aplikacije sustava Office
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
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747768"
---
# <a name="control-automatic-updates-for-office-apps"></a>Kontrola automatskih ažuriranja za aplikacije sustava Office

Ažuriranja za aplikacije sustava Office po zadanom se preuzimaju automatski i primjenjuju u pozadini bez ikakvih intervencija korisnika. No administratori mogu kontrolirati kako se ažuriranja primjenjuju pomoću postavki sustava Office Update. Postavke ažuriranja administratorima omogućuju Omogućivanje i onemogućivanje automatskih ažuriranja, prikazivanje ili sakrivanje gumba **Ažuriraj sada** u sustavu Office, postavljanje rokova ažuriranja i još mnogo toga. Detaljne informacije potražite u članku:

- [Konfiguriranje postavki ažuriranja za Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatsko ažuriranje za Office nije omogućeno](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definiranje načina ažuriranja sustava Office nakon instalacije](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Da biste pregledali postojeće postavke ažuriranja primijenjene na klijentsko računalo, slijedite ove korake:

1. Otvorite uređivač registra tako da **počnete**  >  **pokretati**  >  **regedit**.
2. Prijeđite na sljedeće mjesto i pregledajte postavke sustava Office Update:  
    je. HKEY_LOCAL_MACHINE \software\microsoft\office\  
    b. ClickToRun\Configuration

**Notes**  Ako je ključ servisa officemgmtcom postavljen, možda će se prikazati poruka "ažuriranjima upravlja administrator sustava" u ažuriranju Office **Office**  >  **računa**  >  **Office Updates**. Dodatne informacije potražite u članku [upravljanje ažuriranjima aplikacija microsoft 365 pomoću upravitelja konfiguracije programa Microsoft Endpoint](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  