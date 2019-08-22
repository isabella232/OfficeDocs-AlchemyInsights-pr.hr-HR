---
title: Rješavanje problema s uvrštavate Windows uređaja u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559653"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rješavanje problema s uvrštavate Windows uređaja u Microsoft Intune

Pregledajte resurse dolje navedene da riješite problem.
  
Neke uobičajene poruke o pogreškama i razlučivost korake:
  
 **Ne može biti instaliran softver, 0x80cf4017:** Račun certifikat je istekao. Ponovno preuzmite paket PC klijentski softver u Intune administratorske konzole. Pregledajte dokumentaciju za dodatne informacije.
  
 **0x801c0003 Šifra pogreške:** Pogreška se može pojaviti u sljedećim scenarijima:
  
1. Korisnik ima više uređaja upisani od ograničenja uređaja. Pregledajte te dokumente [ukloniti uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijeniti ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

2. "Korisnici možda pridružite uređaji Azure AD" postavite na "none". Postavljanje svim ili odaberite korisnika. Pregledajte [ove dokumentacije](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za dodatne informacije.

3. Uređaj već upisani drugi korisnik. Ako je to slučaj, uklonite uređaj iz konzole Azure Intune ili ručno unenroll uređaja prije ponovnog pokušaja.

4. Uređaj je Windows 10 Home. Samo Windows 10 Pro, obrazovanje i Enterprise JSK možete pridružiti Azure Active Directory.

Dodatne resurse za pomoć riješiti vaš problem:
  
1. Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene neuspjeha uvrštenje. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.

2. Pregledajte te dokumente za popis uobičajene pogreške koje sprječavaju uvrštenje i rješenja za svaki: [Vodič za otklanjanje poteškoća](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Otklanjanje poteškoća doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Saznajte kako da biste uvrstili Windows uređaja u Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
