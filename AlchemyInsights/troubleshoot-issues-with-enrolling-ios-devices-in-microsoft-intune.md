---
title: Otklanjanje poteškoća s upisom iOS uređaja u Microsoft Intune
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506913"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Otklanjanje poteškoća s upisom iOS uređaja u Microsoft Intune

Pregledajte dolje navedene resurse da biste sada riješili problem. 
  
Neke uobičajene poruke o pogrešci i koraci rezolucije:
  
- **Dosegnut zatvarač uređaja** Korisnik ima više uređaja uključenih od ograničenja uređaja. Pregledajte ove dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ova usluga nije podržana. Nema pravila o prijavi:** Apple push, usluga obavješćivanja (APNS) treba konfigurirati ili obnoviti. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) za upute o tome kako to učiniti. 
    
- **Vrsta licence za korisnika nije valjana ili korisničko ime nije prepoznano:** Korisniku treba dodijeliti licencu Intune ili EMS. Pregledajte ove dokumente da biste dodijelili licencu putem: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) ili [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatni resursi koji pomažu u rješavanju problema:
  
1. Koristite [Intune otklanjanje poteškoća portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) za dijagnosticiranje i rješavanje uobičajenih neuspjeha prijave. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja. 
    
2. Pregledajte ove dokumente za popis uobičajenih pogrešaka koje sprječavaju upis i rezoluciju za svaki: [Vodič za otklanjanje poteškoća](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i pri [rješavanju problema](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Saznajte kako upisati iOS uređaje u Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

