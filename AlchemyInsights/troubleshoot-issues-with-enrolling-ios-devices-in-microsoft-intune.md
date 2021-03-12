---
title: Otklanjanje poteškoća s upisivanjem uređaja sa sustavom iOS u programu Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708954"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Otklanjanje poteškoća s upisivanjem uređaja sa sustavom iOS u programu Microsoft Intune

Pregledajte navedene resurse da biste sada riješili problem. 
  
Neke česte poruke o pogreškama i koraci za rješavanje:
  
- **Stigao je poklopac uređaja** Korisnik ima više uključenih uređaja od ograničenja uređaja. Pregledajte ove dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ovaj servis nije podržan. Nema pravilnika o upisu:** servis Apple push notifikacije (APN-ovi) mora biti konfiguriran ili obnovljen. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) radi uputa o tome kako to učiniti. 
    
- **Vrsta korisničke licence nije valjana ili korisničko ime nije prepoznalo:** Korisniku je potrebno dodijeliti licencu za Intune ili EMS. Pregledajte ove dokumente da biste dodijelili licencu putem: [centar za administratore sustava Office](https://docs.microsoft.com/intune/licenses-assign) ili [portal Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatni resursi koji će vam olakšati rješavanje problema:
  
1. Koristite [portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili česte neuspjehe upisa. Dodatne pojedinosti potražite u [ovom dokumentu](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Pregledajte ove dokumente za popis uobičajenih pogrešaka koje sprječavaju upis i rezolucije na svaki: upute za [Otklanjanje poteškoća](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [Otklanjanje poteškoća s liječnikom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. Upute [za upis uređaja sa sustavom iOS u programu Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

