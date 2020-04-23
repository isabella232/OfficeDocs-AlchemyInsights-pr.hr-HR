---
title: Otklanjanje poteškoća s prijavom iOS uređaja u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736150"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Otklanjanje poteškoća s prijavom iOS uređaja u Microsoft Intune

Pregledajte dolje navedene resurse da biste riješili problem. 
  
Neke uobičajene poruke o pogreškama i koraci rješenja:
  
- **Dosegnuta je gornja granica uređaja** Korisnik ima više uređaja prijavljenih od ograničenja uređaja. Pregledajte te dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ova usluga nije podržana. Nema pravila za prijavu:** Appleovu uslugu obavještavanja o pushu (APNS) potrebno je konfigurirati ili obnoviti. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) za upute o tome kako to učiniti. 
    
- **Vrsta licence korisnika nije valjana ili korisničko ime nije prepoznato:** Korisniku treba dodijeliti Intune ili EMS licencu. Pregledajte te dokumente da biste dodijelili licencu putem: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) ili Portal [azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatni resursi koji će vam pomoći u rješavanju problema:
  
1. Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene pogreške pri upisu. Dodatne informacije potražite [u ovom dokumentu.](https://docs.microsoft.com/intune/help-desk-operators) 
    
2. Pregledajte te dokumente za popis uobičajenih pogrešaka koje sprječavaju prijavu i rješenja za svaku: [Vodič za otklanjanje poteškoća](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i Otklanjanje poteškoća [.](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)
    
3. [Saznajte kako prijaviti iOS uređaje u microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

