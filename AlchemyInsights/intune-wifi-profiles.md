---
title: Intune Wi-Fi profili
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554857"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi profili

Uspješna implementacija Wi-Fi veze za MDM klijente ovisi o ispravno uvedenom profilu koji odražava zahtjeve korporacijske Wi-Fi infrastrukture. Da biste pregledali odgovarajuće postavke za klijentske platforme koje istražujete, pogledajte: 

[Dodavanje Wi-Fi postavki za uređaje sa sustavom Android u programu Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Dodavanje Wi-Fi postavki za android enterprise namjenske i potpuno upravljane uređaje u programu Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Dodavanje Wi-Fi postavki za iOS i iPadOS uređaje u sustavu Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Dodavanje Wi-Fi postavki za Windows 10 i novije uređaje u aplikaciji Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Uvoz Wi-Fi postavki za uređaje sa sustavom Windows u intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Uobičajena pitanja**

**Uvodim Wi-Fi profil koji ovisi o implementiranom certifikatu navedenom u Wi-Fi profilu. Međutim, konfiguracijski profili prikazuju status pogreške.**

Provjerite je li uređaj primio certifikat.

1. U odjeljku Intune idite na **Svi uređaji** i odaberite uređaj > **konfiguracija uređaja**.

2. Provjerite jesu li navedeni svi očekivani profili i u uspješnom stanju.

3. Za Android profil, ako imate međurezultate u lancu certifikata, provjerite jesu li implementirani na Android uređaje.

    Da biste provjerili status certifikata, idite na **Profili za konfiguraciju uređaja**  >  **Profiles**  >  **Android srednji CA**  >  **Properties**  >  **Svojstva Pouzdani certifikat**.

Ako se pogreškama i dalje prikazuje, pregledajte odjeljke za postupke i otklanjanje poteškoća. Dodatne informacije potražite u [odjeljku Pregled otklanjanja poteškoća s profilima certifikata SCEP-a pomoću programa Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Implementirao sam Wi-Fi profil na uređaj. Intune pokazuje da je bio uspješan, ali uređaj se ne povezuje s Wi-Fi.**

Uspješan status znači da je Intune uspješno uveo profil kao konfiguriran. Međutim, te konfiguracije možda ne odgovaraju vašim zahtjevima mreže i/ili provjere autentičnosti. Dodatne informacije o pokušaju povezivanja pregledajte zapisnike u infrastrukturi i servisu za provjeru autentičnosti (na kontroleru točke Wi-Fi pristup i NPS/Radius poslužitelju). Možda ćete morati surađivati s timom za mrežnu infrastrukturu ili dobavljačem Wi-Fi-ja treće strane da biste prikupili i pregledali zapisnike.