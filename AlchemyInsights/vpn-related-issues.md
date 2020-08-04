---
title: Problemi povezani s VPN-om
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554773"
---
# <a name="vpn-related-issues"></a>Problemi povezani s VPN-om

Uspješna implementacija VPN veze za MDM klijente ovisi o implementiranom profilu koji ispravno odražava zahtjeve VPN infrastrukture. Za odgovarajuće postavke za klijentske platforme koje istražujete potražite u članku: 

[Postavke uređaja Windows 10 i Windows Holografski za dodavanje VPN veza pomoću aplikacije Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Dodavanje VPN postavki na iOS i iPadOS uređajima u programu Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Postavke Android uređaja za konfiguriranje VPN-a u intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Dodavanje VPN postavki na macOS uređajima u programu Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Ako vaš VPN profil koristi provjeru autentičnosti na temelju certifikata, provjerite jesu li korijenski certifikat i profili certifikata za provjeru autentičnosti klijenta povezani s VPN profilom uspješno uvedeni.

**Uobičajena pitanja**

**Implementirao sam VPN profil na uređaj. Intune pokazuje da je bio uspješan, ali uređaj se ne povezuje s VPN-om.**

Uspješan status znači da je Intune uspješno uveo profil kao konfiguriran. Međutim, te konfiguracije možda ne odgovaraju vašim zahtjevima mreže i/ili provjere autentičnosti. Pregledajte zapisnike u infrastrukturi i servisu za provjeru autentičnosti (na VPN poslužitelju i NPS/Radius poslužitelju) za više pojedinosti o pokušaju povezivanja. Možda ćete morati surađivati s timom za mrežnu infrastrukturu ili dobavljačem VPN-a treće strane da biste prikupili i pregledali zapisnike.

**Kada konfiguriram prilagođeni VPN za iOS, vpn značajka po aplikaciji nije dostupna.**

VPN po aplikaciji za iOS uređaje u aplikaciji Intune trenutno je dostupan na određenom popisu davatelja i partnera, koji također moraju ispuniti preduvjete certifikata prije konfiguriranja VPN-a po aplikaciji. Dodatne informacije [potražite u odjeljku Postavljanje virtualne privatne mreže (VPN) po aplikaciji za iOS/iPadOS uređaje u aplikaciji Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Dodatne informacije o svim vrstama VPN veza u intune potražite u [odjeljku Stvaranje VPN profila za povezivanje s VPN poslužiteljima u intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**IOS on-Demand VPN ne pokreće kada se pristupa konfiguriranoj domeni**

Da biste testirali automatske POSTAVKE VPN-a, postavite sljedeće vrijednosti:

Želim učiniti sljedeće: **Procijenite svaki pokušaj povezivanja** 

Odaberite želite li se povezati: **Povežite se ako je potrebno**

Kada korisnici pristupaju tim domenama: **ciljni** *naziv domene*

Ako gore navedena konfiguracija nije uspješna, dodajte sljedeći element:

Kada je ovaj URL nedostupan, prisilno povežite VPN: **BADURL**