---
title: Rješavanje problema s uvrštavate Windows uređaja u Microsoft Intune
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665824"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rješavanje problema s uvrštavate Windows uređaja u Microsoft Intune

Pregledajte resurse dolje navedene da riješite problem.
  
Neke uobičajene poruke o pogreškama i razlučivost korake:
  
 **Ne može biti instaliran softver, 0x80cf4017:** Račun certifikat je istekao. Ponovno preuzmite paket PC klijentski softver u Intune administratorske konzole. Pregledajte dokumentaciju za dodatne informacije.
  
 **0x801c0003 Šifra pogreške:** Pogreška se može pojaviti u sljedećim scenarijima:
  
-  Korisnik ima više uređaja upisani od ograničenja uređaja. Pregledajte te dokumente [ukloniti uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijeniti ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Korisnici možda pridružite uređaji Azure AD" postavljen na "none". Postavljanje svim ili odaberite korisnika. Pregledajte [ove dokumentacije](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za dodatne informacije.

-  Uređaj već upisani drugi korisnik. Ako je to slučaj, uklonite uređaj iz konzole Azure Intune ili ručno unenroll uređaja prije ponovnog pokušaja.

-  Uređaj je Windows 10 Home. Samo Windows 10 Pro, obrazovanje i Enterprise JSK možete pridružiti Azure Active Directory.

Dodatne resurse za pomoć riješiti vaš problem:
  
-  Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene neuspjeha uvrštenje. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.

-  Pregledajte te dokumente za popis uobičajene pogreške koje sprječavaju uvrštenje i rješenja za svaki: [Vodič za otklanjanje poteškoća](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Otklanjanje poteškoća doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Saznajte kako da biste uvrstili Windows uređaja u Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
