---
title: Problemi povezani s VPN-om
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
- "1545"
- "9000076"
ms.openlocfilehash: 1d9c34350d16d96329d1ed56666119dba0433c93ccb7547da5dba4894531e1b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53970971"
---
# <a name="vpn-related-issues"></a>Problemi povezani s VPN-om

Uspješna implementacija VPN povezivanja za KLIJENTE MDM-a ovisi o implementiranom profilu koji pravilno odražava preduvjete VPN infrastrukture. Odgovarajuće postavke za klijentske platforme koje istražujete nalaze se u odjeljku: 

[Windows 10 i Windows holografskih uređaja za dodavanje VPN veza pomoću aplikacije Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Dodavanje POSTAVKI VPN-a na uređajima sa sustavom iOS i iPadOS Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Postavke uređaja sa sustavom Android za konfiguriranje VPN-a u aplikaciji Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Dodavanje POSTAVKI VPN-a na uređajima sa sustavom macOS Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Ako vpn profil koristi provjeru autentičnosti utemeljenu na certifikatu, provjerite jesu li korijenski certifikat i profili certifikata za provjeru autentičnosti klijenta povezani s VPN profilom uspješno implementiran.

**Uobičajeni problemi**

**Implementiran sam VPN profil na uređaj. Intune pokazuje da je bio uspješan, ali se uređaj ne povezuje s VPN-om.**

Uspješan status znači da je Intune uspješno implementirao profil kao konfiguriran. No te konfiguracije možda ne odgovaraju vašim mrežnim i/ili preduvjetima za provjeru autentičnosti. Pregledajte zapisnike u servisu za infrastrukturu i provjeru autentičnosti (na VPN poslužitelju i poslužitelju NPS/Radius) da biste saznali više o pokušaju povezivanja. Možda ćete morati raditi s timom za mrežnu infrastrukturu ili dobavljačem VPN-a drugih proizvođača da biste prikupili i pregledali zapisnike.

**Kada konfiguriram prilagođeni VPN za iOS, značajka VPN-a po aplikaciji nije dostupna.**

VPN za iOS uređaje u aplikaciji Intune trenutno je dostupan određenom popisu davatelja i partnera koji moraju zadovoljiti preduvjete certifikata prije konfiguriranja VPN-a po aplikaciji. Dodatne informacije potražite u članku Postavljanje virtualne privatne mreže (VPN- a) za uređaje sa sustavom [iOS/iPadOS u aplikaciji Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Dodatne informacije o svim vrstama VPN veza u aplikaciji Intune potražite u članku Stvaranje VPN profila za povezivanje s [VPN poslužiteljima u aplikaciji Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**VPN za iOS na zahtjev ne pokreće se kada se pristupa konfiguriranoj domeni**

Da biste testirajte automatske postavke VPN-a, postavite sljedeće vrijednosti:

Želim učiniti sljedeće: procjena **svakog pokušaja povezivanja** 

Odaberite želite li se povezati: **Povezivanje po potrebi**

Kada korisnici pristupaju tim domenama: **naziv ciljne** *domene*

Ako gore navedena konfiguracija nije uspješna, dodajte sljedeći element:

Kada url nije dostupan, prisilno povežite VPN: **BADURL**