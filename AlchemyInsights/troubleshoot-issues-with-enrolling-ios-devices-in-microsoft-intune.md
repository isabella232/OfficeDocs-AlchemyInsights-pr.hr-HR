---
title: Otklanjanje poteškoća s prijavom uređaja sa sustavom iOS u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047968"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Otklanjanje poteškoća s prijavom uređaja sa sustavom iOS u Microsoft Intune

Pregledajte resurse navedene u nastavku da biste odmah riješili problem. 
  
Neke uobičajene poruke o pogreškama i koraci za rješavanje:
  
- **Dosegnut je cap device cap** Korisnik ima više uređaja koji su upisani od ograničenja uređaja. Pregledajte te [dokumente da biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) [ili promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ovaj servis nije podržan. Bez pravilnika za prijavu:** Appleov servis za automatsko obavještavanje (APNS) mora se konfigurirati ili obnoviti. Upute [za to](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) potražite u ovom dokumentu. 
    
- **Vrsta korisničke licence nije valjana ili korisničko ime nije prepoznato:** Korisniku je potrebno dodijeliti licencu za Intune ili EMS. Pregledajte ove dokumente da biste dodijelili licencu putem: [Office centra za administratore ili](https://docs.microsoft.com/intune/licenses-assign) [portala Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatni resursi za rješavanje problema:
  
1. Pomoću [portala za otklanjanje poteškoća sa servisom Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) dijagnosticirajte i riješite uobičajene pogreške prilikom prijave. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) da biste saznali više. 
    
2. Pregledajte ove dokumente da biste pregledali popis uobičajenih pogrešaka koje sprječavaju prijavu i rješenja za svaku od njih: vodič za otklanjanje [poteškoća i dokument](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) za otklanjanje [poteškoća.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Saznajte kako registrirati uređaje sa sustavom iOS u Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

