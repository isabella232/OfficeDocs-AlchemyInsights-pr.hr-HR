---
title: Intune Wi-Fi profile
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: 5e5258806c8a38965467a8878bc8ac922c2668f21abe3602f479dcdaff8c9b5b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028212"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi profile

Uspješna implementacija Wi-Fi za MDM klijente ovisi o pravilno implementiranom profilu koji odražava zahtjeve korporativne Wi-Fi infrastrukture. Da biste pregledali odgovarajuće postavke za klijentske platforme koje istražujete, pogledajte sljedeće: 

[Dodavanje Wi-Fi za uređaje sa sustavom Android u Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Dodavanje Wi-Fi za namjenske uređaje namijenjene za Android Enterprise i potpuno upravljane uređaje u Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Dodavanje Wi-Fi za uređaje sa sustavom iOS i iPadOS u Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Dodavanje Wi-Fi za Windows 10 i novijim uređajima u aplikaciji Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Uvoz Wi-Fi za Windows u aplikaciji Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Uobičajeni problemi**

**Implementiram profil Wi-Fi koji ovisi o implementiranom certifikatu navedenom u profilu Wi-Fi. No konfiguracijski profili prikazuju status pogreške.**

Provjerite je li vaš uređaj primio certifikat.

1. U aplikaciji Intune idite **na Svi uređaji** i odaberite uređaj > konfiguracija **uređaja**.

2. Provjerite jesu li svi očekivani profili navedeni i u uspješnom stanju.

3. Ako imate posredne certifikate u lancu certifikata, provjerite jesu li implementirane na uređaje sa sustavom Android.

    Da biste provjerili status certifikata, idite na **Profili konfiguracije**  >  **uređaja**  >  **Za Android posredni CA**  >  **svojstva**  >  **pouzdani certifikat**.

Ako i dalje vidite pogreške, pregledajte postupke i odjeljke za otklanjanje poteškoća. Dodatne informacije potražite u članku Pregled [otklanjanja poteškoća s profilima SCEP certifikata Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Implementiran sam Wi-Fi na uređaj. Intune pokazuje da je bio uspješan, ali se uređaj ne povezuje s Wi-Fi mrežom.**

Uspješan status znači da je Intune uspješno implementirao profil kao konfiguriran. No te konfiguracije možda ne odgovaraju vašim mrežnim i/ili preduvjetima za provjeru autentičnosti. Dodatne informacije o pokušaju povezivanja potražite u zapisnicima u infrastrukturnom servisu i servisu za provjeru autentičnosti (na kontroleru Wi-Fi pristupne točke i poslužitelju NPS/Radius). Da biste prikupili i pregledali zapisnike, možda ćete morati raditi s timom za mrežnu infrastrukturu ili Wi-Fi proizvođačem.