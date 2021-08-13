---
title: Otklanjanje poteškoća s prijavom uređaja sa sustavom Android u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008070"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Otklanjanje poteškoća s prijavom uređaja sa sustavom Android u Microsoft Intune

Pregledajte resurse navedene u nastavku da biste odmah riješili problem.
  
Neki uobičajeni problemi i koraci za rješavanje:
  
 **Pogreška uređaja nije šifrirana u Company Portal:** Novije verzije sustava Android, osobito počevši od verzije v7.0, zahtijevaju pristupnu šifru za pokretanje da biste bili sigurni da je uređaj u potpunosti šifriran. Uobičajena su rješenja omogućivanje pribadače za pokretanje ili potpuno šifriranje uređaja. Dodatne [informacije potražite](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) u ovom dokumentu.
  
 **Uređaji se ne prijave pomoću servisa Intune ili se prikazuju kao "nezdravi" na administratorskim konzolama aplikacije Intune:** Neki uređaji Samsung 4.4 i 5.5 možda se ne prijave u servis. Za taj problem postoje tri moguća rješenja:
  
1. Ručno otvorite aplikaciju Intune Company Portal, koja će automatski pokrenuti sinkronizaciju uređaja.

2. Ažurirajte uređaj na Android 6.0 ili noviji.

3. Onemogućite Samsung Smart Manager da upravlja Intune Company Portal. Pregledajte [ovaj dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) da biste vidjeli dodatne pojedinosti o tim problemima i rješavanjima.

 **Pogreška Vrsta korisničke licence nije** **valjana ili** korisničko ime nije prepoznato: korisniku je potrebno dodijeliti licencu za Intune ili EMS. Pregledajte ove dokumente da biste dodijelili licencu putem: Office centra za administratore ili portala Azure.
  
Dodatni resursi za rješavanje problema:
  
1. Pomoću [portala za otklanjanje poteškoća sa servisom Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) dijagnosticirajte i riješite uobičajene pogreške prilikom prijave. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) da biste saznali više.

2. Pregledajte [ovaj dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) da biste pregledali popis uobičajenih pogrešaka koje sprječavaju registraciju i rješenja za svaku od njih.

3. [Saznajte kako registrirati uređaje sa sustavom Android u Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
