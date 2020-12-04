---
title: Otklanjanje poteškoća s izdankom PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573380"
---
# <a name="troubleshoot-prt-issue"></a>Otklanjanje poteškoća s izdankom PRT

Da bi bilo koji uređaj trebao biti autentičan, mora biti u potpunosti registriran i u dobroj državi i može steći primarni token osvježavanja (PRT).

Postupak registracije za hibridnu verziju Azure AD Join zahtijeva da uređaji budu na korporacijskom mreži. Internet isto tako utvrde na VPN, ali ima neki opomena to taj. Čuli smo da kupci trebaju pomoć pri otklanjanju poteškoća s postupkom registracije hibridne Azure AD Join u odjeljku uvjeti daljinskog rada. Ovdje se nalazi slom događaja "Under The Hood" tijekom postupka registracije.

**Okruženje za provjeru autentičnosti u oblaku (korištenje značajke korištenja lozinke za Azure AD i provjera autentičnosti)**

Ovaj tijek registracije poznat je i kao "Sinkronizacija pridruživanja".

1. Windows 10 otkriva zapis o SCP-u na korisniku koji se prijavljuje na uređaj.
    1. Uređaj najprije pokuša dohvatiti informacije o klijentu s klijentskog SCP-a u registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Ako ne uspije, uređaj komunicira s lokalnim servisom Active Directory (AD) da bi dobio informacije o klijentu iz točke veze za servis (SCP). Da biste potvrdili SCP, pogledajte ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Preporučujemo vam da u OGLASU omogućite SCP, a za početnu provjeru valjanosti koristite samo SKP na strani klijenta.

2. Windows 10 pokušava razgovarati s Azure AD u odjeljku sistemski kontekst radi provjere autentičnosti za Azure AD. Možete potvrditi može li uređaj pristupati Microsoftovim resursima u odjeljku sistemski račun pomoću skripte za povezivanje s registriranjem testnog uređaja.

3. Windows 10 generira samopotpisani certifikat i pohranjuje ga ispod objekta računala u lokalnom AD-u. Za to je potreban kontrolor domene.

4. Objekt uređaja s certifikatom može se sinkronizirati s programom Azure AD putem servisa Azure AD Connect. Ciklus sinkronizacije svaki je 30 minuta po zadanom, ali ovisi o konfiguraciji servisa Azure AD Connect. Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. U ovoj će fazi biti moguće vidjeti predmet uređaja u odjeljku "u tijeku" u odjeljku sprava Blade of Azure portal.

6. Kada se sljedeći korisnik prijavi na Windows 10, registracija će biti dovršena. 

> [!NOTE]
> Ako ste na VPN-u, a ako je postupak prijave neograničen, možete ručno pokrenuti registraciju:
 1. Izdanje dsregcmd/pridružite se lokalno na administratorskom upitu ili na daljinu putem Psexez-a na PC. Na primjer, Psexez-s \\ win10client01 cmd, dsregcmd/Join

 2. Dodatne informacije o hibridnim pitanjima pridruživanja potražite u članku [Otklanjanje poteškoća s uređajima](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
