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
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726083"
---
# <a name="vpn-related-issues"></a>Problemi povezani s VPN-om

Uspješna implementacija VPN povezivosti za klijente MDM-a zavisi od raspoređenih profila koji pravilno odražava zahtjeve VPN infrastrukture. Odgovarajuće postavke za klijentsku platformu koju istražujete potražite u članku: 

[Windows 10 i Windows holo-postavke uređaja za dodavanje VPN veza pomoću aplikacije Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Dodavanje VPN postavki na uređajima sa sustavom iOS i iPadOS u programu Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Postavke uređaja sa sustavom Android da biste konfigurirali VPN u programu Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Dodavanje VPN postavki na uređajima macOS u programu Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Ako vaš VPN profil koristi provjeru autentičnosti utemeljenu na certifikatu, provjerite jesu li korijenski certifikat i profili certifikata za provjeru autentičnosti povezani s VPN profilom uspješno razmješteni.

**Česti problemi**

**Rasporedio sam VPN profil na uređaj. Intune pokazuje da je bila uspješna, no uređaj se ne povezuje s VPN-ovim.**

Uspješan status znači da je Intune uspješno implementirao profil kao konfiguriran. No te se konfiguracije možda neće podudarati s vašim zahtjevima za mrežu i/ili provjeru autentičnosti. Pregled zapisnika u servisu za infrastrukturu i provjeru autentičnosti (na poslužitelju VPN poslužitelja i NPS/radius Server) dodatne informacije o pokusaju povezivanja. Možda ćete morati raditi s tim mrežnim infrastrukturom ili drugim proizvođačima VPN-a, da biste prikupili i pregledavali zapisnike.

**Kada Konfiguriram prilagođeni VPN za iOS, značajka VPN-a po aplikaciji nije dostupna.**

VPN-ovi za uređaje sa sustavom iOS u programu Intune na aplikaciji trenutno su dostupni određenom popisu pružatelja usluga i partnera, koji moraju zadovoljiti preduvjete certifikata prije konfiguriranja VPN-a po aplikaciji. Dodatne informacije potražite u članku [Postavljanje virtualne privatne mreže (VPN-a) za iOS/iPadOS uređaje u aplikaciji Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Dodatne informacije o svim vrstama VPN veza u programu Intune potražite u članku [Stvaranje VPN profila za povezivanje s VPN poslužiteljima u programu Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**VPN na servisu iOS na zahtjev ne pokreće se kada se pristupi konfiguriranoj domeni**

Da biste testirali automatske VPN postavke, postavite sljedeće vrijednosti:

Želim učiniti sljedeće: **procijeniti svaki pokušaj povezivanja** 

Odaberite želite li se povezati: **povezivanje ako je potrebno**

Kada korisnici pristupe ovim domenama: **Odredišni** *naziv domene*

Ako gore navedena konfiguracija nije uspješna, dodajte sljedeći element:

Kada taj URL nije dostupan, silom povežite VPN: **Badurl**