---
title: Rješavanje problema s uvrštavate Android uređaja Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655875"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Rješavanje problema s uvrštavate Android uređaja Microsoft Intune

Pregledajte resurse dolje navedene da riješite problem.
  
Neke uobičajene probleme i rješenja korake:
  
 **Uređaj nije šifrirana pogreška u poduzeću Portal:** Novije verzije Android, osobito počevši s v7.0, zahtijevaju pokretanje "passcode" da biste bili sigurni da uređaj u potpunosti šifrirana. Da biste omogućili pin za pokretanje ili potpuno šifriranje uređaj su uobičajene rješenja. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) dodatne informacije. 
  
 **Uređaji neće uspjeti za provjeru pomoću servisa Intune ili prikazati kao "Unhealthy" u administratorske konzole Intune:** Neke 4.4 Samsung i 5.5 uređaji možda provjerite u servis. Postoje 3 mogućih rješenja za ovaj problem: 
  
1. Ručno otvaranje app Portal tvrtke Intune koji će automatski započeti sinkronizaciju uređaja.
    
2. Ažuriranje uređaja na Android 6.0 ili noviji.
    
3. Onemogući upravitelja pametne Samsung iz upravljanje Portal tvrtke Intune. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za daljnje pojedinosti o ti problemi i rješenja. 
    
 **Korisničke licence vrsta valjan** ili **korisničko ime nije prepoznato pogreška:** korisnik mora biti dodijeljen Intune ili EMS licence. Pregledajte te dokumente dodeljivanje licence kroz: Office Admin centar ili Azure portal. 
  
Dodatne resurse za pomoć riješiti vaš problem:
  
1. Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene neuspjeha uvrštenje. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja. 
    
2. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za popis uobičajene pogreške koje sprječavaju uvrštenje i rješenja za svaki. 
    
3. [Saznajte kako da biste uvrstili Android uređaja Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
    

