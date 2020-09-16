---
title: Intune Wi-Fi profili
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
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696253"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi profili

Uspješna implementacija Wi-Fi veze za klijente MDM-a ovisi o pravilno raspoređeni profil koji odražava preduvjete korporativnih Wi-Fi infrastrukture. Da biste pregledali odgovarajuće postavke za klijentske platforme koje istražujete, pročitajte sljedeće: 

[Dodavanje Wi-Fi postavki za uređaje sa sustavom Android u programu Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Dodavanje Wi-Fi postavki za tvrtke sa sustavom Android i potpuno upravljanih uređaja u programu Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Dodavanje Wi-Fi postavki za uređaje sa sustavom iOS i iPadOS u programu Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Dodavanje Wi-Fi postavki za uređaje sa sustavom Windows 10 i novije verzije u programu Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Uvoz Wi-Fi postavki za uređaje sa sustavom Windows u programu Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Česti problemi**

**Implementiram Wi-Fi profil koji ovisi o raspoređenim certifikatu navedenom u profilu Wi-Fi. No profili za konfiguraciju prikazuju status pogreške.**

Provjerite je li vaš uređaj primio certifikat.

1. U programu Intune otvorite **sve uređaje** i odaberite uređaj > **konfiguraciji uređaja**.

2. Provjerite jesu li svi očekivani profili navedeni i u uspješnom stanju.

3. Ako imate profil za Android, ako imate posredne certifikate u lancu certifikata, provjerite jesu li razmješteni na uređaje sa sustavom Android.

    Da biste provjerili status certifikata, idite na **profile konfiguracije uređaja**  >  **Profiles**  >  **Android Intermedijarni**  >  **Properties**  >  **certifikat**za svojstva.

Ako i dalje vidite pogreške, pregledajte procedure i sekcije otklanjanja poteškoća. Dodatne informacije potražite u članku [Pregled rješenja otklanjanja poteškoća s profilima certifikata u programu Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Rasporedio sam Wi-Fi profil na uređaj. Intune pokazuje da je bila uspješna, no uređaj se ne povezuje s Wi-Fi-jem.**

Uspješan status znači da je Intune uspješno implementirao profil kao konfiguriran. No te se konfiguracije možda neće podudarati s vašim zahtjevima za mrežu i/ili provjeru autentičnosti. Dodatne informacije o pokusaju veze potražite u evidenciji za infrastrukturu i provjeru autentičnosti (na kontroleru za Wi-Fi Access Point i NPS/radius Server). Možda ćete morati raditi s tim mrežnim infrastrukturom ili drugim dobavljačima wi-fija, da biste prikupili i pregledavali zapisnike.