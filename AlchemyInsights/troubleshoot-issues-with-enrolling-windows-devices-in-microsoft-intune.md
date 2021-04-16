---
title: Otklanjanje poteškoća s registracijom uređaja sa sustavom Windows u aplikaciji Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808963"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Otklanjanje poteškoća s registracijom uređaja sa sustavom Windows u aplikaciji Microsoft Intune

Pregledajte resurse navedene u nastavku da biste odmah riješili problem.
  
Neke uobičajene poruke o pogreškama i koraci za rješavanje:
  
 **Softver nije moguće instalirati, 0x80cf4017:** Vaš je certifikat računa istekao. Ponovno preuzmite softverski paket klijentskog računala na konzoli za administratore aplikacije Intune. Dodatne informacije potražite u ovoj dokumentaciji.
  
 **Kod pogreške 0x801c0003:** Pogreška se može pojaviti u sljedećim scenarijima:
  
-  Korisnik ima više uređaja koji su upisani od ograničenja uređaja. Pregledajte te [dokumente da biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) [ili promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Korisnici se mogu pridružiti uređajima na servisu Azure AD" postavljen je na "none". Postavite je na sve ili odaberite korisnike. Dodatne [informacije potražite](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) u ovoj dokumentaciji.

-  Uređaj je već prijavio drugi korisnik. U tom slučaju uklonite uređaj s konzole Azure Intune ili ručno poništite zahtjev uređaja prije nego što ga ponovno počnete pokušavati.

-  Uređaj je Windows 10 Home. Samo SKU-i za Windows 10 Pro, Education i Enterprise mogu se pridružiti servisu Azure Active Directory.

Dodatni resursi za rješavanje problema:
  
-  Pomoću [portala za otklanjanje poteškoća sa servisom Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) dijagnosticirajte i riješite uobičajene pogreške prilikom prijave. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) da biste saznali više.

-  Pregledajte ove dokumente da biste pregledali popis uobičajenih pogrešaka koje sprječavaju prijavu i rješenja za svaku od njih: vodič za otklanjanje [poteškoća i dokument](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) za otklanjanje [poteškoća.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Saznajte kako registrirati uređaje sa sustavom Windows u aplikaciji Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
