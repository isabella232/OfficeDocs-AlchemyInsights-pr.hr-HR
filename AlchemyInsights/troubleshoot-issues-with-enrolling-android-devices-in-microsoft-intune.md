---
title: Otklanjanje poteškoća s upisivanjem uređaja sa sustavom Android u programu Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689946"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Otklanjanje poteškoća s upisivanjem uređaja sa sustavom Android u programu Microsoft Intune

Pregledajte navedene resurse da biste sada riješili problem.
  
Neki Česti problemi i koraci sanacije:
  
 **Pogreška uređaja nije šifrirana na portalu tvrtke:** Novije verzije sustava Android, posebno Počevši od v 7.0, zahtijevaju lozinku za pokretanje da biste provjerili je li vaš uređaj potpuno šifriran. Najčešća rješenja jesu omogućivanje PIN-a za pokretanje ili potpuno šifriranje uređaja. Dodatne informacije potražite u [ovom dokumentu](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .
  
 **Uređaji se ne mogu prijaviti pomoću servisa Intune ili prikaza kao "nezdravih" u konzoli za administratore:** Neki uređaji za Samsung 4,4 i 5,5 možda se neće prijaviti u servis. U ovom problemu postoje tri moguća rješenja:
  
1. Ručno otvorite aplikaciju Intune Company portal koja će automatski pokrenuti sinkronizaciju uređaja.

2. Ažurirajte uređaj na Android 6,0 ili noviji.

3. Onemogućite Samsung Smart Manager da upravlja putem portala Intune Company. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) da biste saznali više o tim pitanjima i rezolucijama.

 **Vrsta korisničke licence nije valjana** ili **korisničko ime nije prepoznata pogreška:** korisniku je potrebno dodijeliti licencu za Intune ili EMS. Pregledajte ove dokumente da biste dodijelili licencu putem: centar za administratore sustava Office ili portal Azure.
  
Dodatni resursi koji će vam olakšati rješavanje problema:
  
1. Koristite [portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili česte neuspjehe upisa. Dodatne pojedinosti potražite u [ovom dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .

2. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) radi popisa uobičajenih pogrešaka koji sprječavaju upis i rezolucije na svaki od njih.

3. Upute [za upis uređaja sa sustavom Android u programu Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
