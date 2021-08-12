---
title: Otklanjanje poteškoća s PRT-om
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
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972708"
---
# <a name="troubleshoot-prt-issue"></a>Otklanjanje poteškoća s PRT-om

Da bi bilo koji uređaj dovršio provjeru autentičnosti, mora biti u potpunosti registriran i u dobrom stanju i moći nabaviti token primarnog osvježavanja (PRT).

Hibridni postupak registracije za pridruživanje servisa Azure AD zahtijeva da se uređaji u poslovnoj mreži. Funkcionira i nad VPN-om, ali postoje neke upozorenje o tome. Čuli smo da korisnicima treba pomoć pri otklanjanju poteškoća s hibridnim postupkom registracije pridruživanja servisa Azure AD u okolnostima udaljenog rada. Evo što se događa "ispod haube" tijekom postupka registracije.

**Okruženje za provjeru autentičnosti u oblaku (pomoću sinkronizacije i provjere autentičnosti lozinke za Azure AD)**

Taj je tijek registracije poznat i kao "Sinkronizacija spoja".

1. Windows 10 otkrije SCP zapis nakon prijave korisnika na uređaj.
    1. Uređaj najprije pokušava dohvatiti podatke klijenta iz klijentskog SCP-a u registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Ako ne uspije, uređaj komunicira s lokalnim servisom Active Directory (AD) radi primanja podataka o klijentu iz točke povezivanja servisa (SCP). Da biste potvrdili SCP, pogledajte [ovaj dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> Preporučujemo da omogućite SCP u AD-u i koristite samo klijentski SCP za početnu provjeru valjanosti.

2. Windows 10 pokušava komunicirati sa servisom Azure AD u kontekstu sustava da bi se provjerila autentičnost u odnosu na Azure AD. Možete provjeriti može li uređaj pristupiti Microsoftovim resursima putem računa sustava pomoću skripte Test Device Registration Connectivity.

3. Windows 10 generira samoispravni certifikat i pohranjuje ga ispod objekta računala u lokalnom AD-u. Za to je potreban linijski kontroler domene.

4. Objekt uređaja s certifikatom sinkronizira se sa servisom Azure AD putem servisa Azure AD Povezivanje. Ciklus sinkronizacije po zadanom je svakih 30 minuta, ali ovisi o konfiguraciji servisa Azure AD Povezivanje. Dodatne informacije potražite u ovom [dokumentu.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. U ovoj fazi trebali biste moći vidjeti predmet uređaja u stanju "Na čekanju" ispod oštrice uređaja portala Azure.

6. Prilikom sljedeće prijave korisnika na Windows 10 registracija će biti dovršena. 

> [!NOTE]
> Ako ste na VPN-u i postupak prijave e-pošte prekida vezu s domenom, registraciju možete pokrenuti ručno:
 1. Problem dsregcmd /join locally on admin prompt or remotely via PSExec to your PC. Na primjer, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Dodatne informacije o problemima hibridnog pridruživanja potražite u članku Otklanjanje [poteškoća s uređajima](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
