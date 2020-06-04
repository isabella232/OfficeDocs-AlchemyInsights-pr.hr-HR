---
title: Otklanjanje poteškoća s prijavom uređaja sa sustavom Windows u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665824"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Otklanjanje poteškoća s prijavom uređaja sa sustavom Windows u Microsoft Intune

Pregledajte resurse navedene u nastavku da biste odmah riješili problem.
  
Neke uobičajene poruke o pogreškama i koraci razlučivosti:
  
 **Softver se ne može instalirati, 0x80cf4017:** Certifikat računa je istekao. Ponovno preuzmite softverski paket PC Klijent u Intune Admin Console. Dodatne informacije potražite u ovoj dokumentaciji.
  
 **Kod pogreške 0x801c0003:** Pogreška se može pojaviti u sljedećim scenarijima:
  
-  Korisnik ima više uređaja upisanih od ograničenja uređaja. Pregledajte te dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Korisnici se mogu pridružiti uređajima azure AD" postavljeno je na "ništa". Postavite ga na sve ili odaberite korisnike. Dodatne informacije potražite [u ovoj dokumentaciji.](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)

-  Uređaj je već upisao drugi korisnik. Ako je to slučaj, uklonite uređaj s konzole Azure Intune ili ručno odete uređaj prije ponovnog pokušaja.

-  Uređaj je Windows 10 Home. Samo SE JSK-ovi za Windows 10 Pro, Education i Enterprise mogu pridružiti servisu Azure Active Directory.

Dodatni resursi koji olakšavaju rješavanje problema:
  
-  [Koristite Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene pogreške u prijavi. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.

-  Pregledajte popis uobičajenih pogrešaka koje sprječavaju prijavu i rješenja u svaki: Vodič za [otklanjanje poteškoća](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i Dokument za [otklanjanje poteškoća](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Saznajte kako prijaviti uređaje sa sustavom Windows u Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
