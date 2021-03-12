---
title: Otklanjanje poteškoća s upisivanjem uređaja sa sustavom Windows u programu Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708882"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Otklanjanje poteškoća s upisivanjem uređaja sa sustavom Windows u programu Microsoft Intune

Pregledajte navedene resurse da biste sada riješili problem.
  
Neke česte poruke o pogreškama i koraci za rješavanje:
  
 **Softver se ne može instalirati, 0x80cf4017:** Potvrda računa je istekla. Ponovno preuzmite računalni programski paket PC-ja u konzoli za administratore. Dodatne informacije potražite u dokumentaciji.
  
 **Kod pogreške 0x801c0003:** Pogreška se može pojaviti u sljedećim scenarijima:
  
-  Korisnik ima više uključenih uređaja od ograničenja uređaja. Pregledajte ove dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Korisnici se mogu pridružiti uređajima za Azure AD" postavljen je na "none". Postavite ga na sve ili odaberite korisnike. Dodatne informacije potražite u [dokumentaciji](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Uređaj je već upisao neki drugi korisnik. Ako je to slučaj, uklonite uređaj iz konzole Azure Intune ili ručno isključite uređaj prije ponovnog pokušaja.

-  Uređaj je Windows 10 home. Samo Windows 10 Pro, Education i Enterprise SKUs mogu se pridružiti Azure Active direktoriju.

Dodatni resursi koji će vam olakšati rješavanje problema:
  
-  Koristite [portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili česte neuspjehe upisa. Dodatne pojedinosti potražite u [ovom dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .

-  Pregledajte ove dokumente za popis uobičajenih pogrešaka koje sprječavaju upis i rezolucije na svaki: upute za [Otklanjanje poteškoća](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Otklanjanje poteškoća s liječnikom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Naučite kako upisati uređaje sa sustavom Windows u programu Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
