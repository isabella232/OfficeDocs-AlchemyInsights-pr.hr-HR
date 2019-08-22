---
title: Rješavanje problema s uvrštavate iOS uređaja u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506913"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Rješavanje problema s uvrštavate iOS uređaja u Microsoft Intune

Pregledajte resurse dolje navedene da riješite problem. 
  
Neke uobičajene poruke o pogreškama i razlučivost korake:
  
- **Dostignuto pokrova uređaja** Korisnik ima više uređaja upisani od ograničenja uređaja. Pregledajte te dokumente [ukloniti uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijeniti ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- Ovaj servis **nije podržana. Nema pravila uvrštenje:** Apple Gurni obavijesti servisa (APN-ove) mora biti konfiguriran ili obnoviti. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) za upute kako to učiniti. 
    
- **Nije valjana vrsta licence korisnika ili korisničko ime nije prepoznata:** Korisnik mora biti dodijeljen Intune ili EMS licence. Pregledajte te dokumente dodeljivanje licence kroz: [Office Admin centar](https://docs.microsoft.com/intune/licenses-assign) ili [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatne resurse za pomoć riješiti vaš problem:
  
1. Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene neuspjeha uvrštenje. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja. 
    
2. Pregledajte te dokumente za popis uobičajene pogreške koje sprječavaju uvrštenje i rješenja za svaki: [Vodič za otklanjanje poteškoća](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [Otklanjanje poteškoća doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Saznajte kako da biste uvrstili iOS uređaja u Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

