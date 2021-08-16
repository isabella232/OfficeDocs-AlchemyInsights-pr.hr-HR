---
title: Otklanjanje poteškoća s implementacijom certifikata za provjeru autentičnosti klijenta
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
- "1546"
- "9000076"
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020796"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Otklanjanje poteškoća s implementacijom certifikata za provjeru autentičnosti klijenta

Profili certifikata NDES/SCEP i PKCS/PFX klijenta intune obično se koriste u kombinaciji s drugim vrstama profila kao što su WiFi, VPN i e-pošta da bi korisnicima omogućili provjeru autentičnosti korporativnih resursa. Kada su te vrste profila povezane s profilom klijentskog certifikata, ovise o uspješnoj implementaciji tog profila.

Početno postavljanje infrastrukture i povezana konfiguracija profila klijentskog certifikata često zahtijevaju otklanjanje poteškoća. Vodič za uspješno postavljanje poveznika za NDES i upute za otklanjanje poteškoća radi izdvajanja problema s implementacijom certifikata možete naći u sljedećem članku: 

- [Konfiguriranje infrastrukture za podršku SCEP-u uz Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Pregled otklanjanja poteškoća s profilima SCEP certifikata Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Pomoću referencijnih skripti ljuske powershell potvrdite konfiguraciju. Dodatne informacije potražite u članku Skripte za [provjeru valjanosti poveznika certifikata intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Ostali uobičajeni problemi**

**Kada pokušam instalirati poveznik intune certifikata na poslužitelj poveznika NDES-a, prikazuje mi se poruka "Lozinka u zahtjevu za certifikat nije moguće provjeriti. Možda se već koristio. Nabavite novu lozinku za slanje s ovim zahtjevom."**  

Ova poruka znači da morate pokrenuti instalaciju poveznika certifikata kao administratora.

U nekim okruženjima poslužitelji na kojima se izvodi Intuneov certifikat moraju koristiti proxy poslužitelj da bi se povezali s programom Intune, pa poveznik certifikata mora koristiti proxy. U nekim okolnostima NDES Connector zanemaruju konfigurirane postavke proxyja i možda će biti potrebno konfigurirati postavke proxyja tijekom rada u sigurnosnom kontekstu localsystema. 
 
Rješenje je pokretanje preglednika Internet Explorer kao sustava i konfiguriranje proxyja u IE-u. Nakon ponovnog pokretanja servisa Intune Connector NDES Connector povezuje se s aplikacijom Intune.

**Korisnički uređaji više ne primaju SCEP certifikate od NDES-a.**

Moguće je da je certifikat za provjeru autentičnosti klijenta izdan NDES poslužitelju i naveden tijekom instalacije poveznika NDES-a istekao ili nedostaje. Da biste riješili problem: 
 
1. Deinstalirajte poveznik za NDES.  
2. Da biste zatražili novu provjeru autentičnosti klijenta ili certifikat za provjeru autentičnosti poslužitelja, upotrijebite ove pojedinosti: 
 
    - Naziv predmeta: CN=external fqdn  
    - Alternativni naziv predmeta (oba su obavezna): DNS=vanjski fqdn, DNS=interni fqdn 
 
3. Ponovno instalirajte NDES poveznik pomoću novog certifikata.