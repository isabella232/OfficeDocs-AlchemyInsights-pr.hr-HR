---
title: Otklanjanje poteškoća s prijavom Android uređaja u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759612"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Otklanjanje poteškoća s prijavom Android uređaja u Microsoft Intune

Pregledajte dolje navedene resurse da biste riješili problem.
  
Neki uobičajeni problemi i koraci rješavanja:
  
 **Uređaj nije šifrirana pogreška na portalu tvrtke:** Novije verzije Androida, osobito počevši od v7.0, zahtijevaju šifru za pokretanje kako bi se osiguralo da je vaš uređaj u potpunosti šifriran. Uobičajena su rješenja omogućiti pribadaču za pokretanje ili potpuno šifrirati uređaj. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) za više informacija.
  
 **Uređaji propust to check in sa Intune poslužitelj ili otkriti kao " nezdrav" in Intune admin utješiti:** Neki uređaji Samsung 4.4 i 5.5 možda se neće prijaviti na uslugu. Postoje 3 moguća rješenja za ovaj problem:
  
1. Ručno otvorite aplikaciju Intune Portal tvrtke koja će automatski pokrenuti sinkronizaciju uređaja.

2. Ažurirajte uređaj na Android 6.0 ili noviji.

3. Onemogućite Samsung Smart Manager u upravljanju portalom tvrtke Intune. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za dodatne pojedinosti o tim pitanjima i rješenjima.

 **Vrsta licence korisnika Nije valjano** ili **korisničko ime nije prepoznato:** korisniku treba dodijeliti Intune ili EMS licencu. Pregledajte te dokumente da biste dodijelili licencu putem: Office Admin Center ili Portal azure.
  
Dodatni resursi koji će vam pomoći u rješavanju problema:
  
1. Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene pogreške pri upisu. Dodatne informacije potražite [u ovom dokumentu.](https://docs.microsoft.com/intune/help-desk-operators)

2. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za popis uobičajenih pogrešaka koje sprječavaju prijavu i rješenja za svaku od njih.

3. [Saznajte kako prijaviti Android uređaje u Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
