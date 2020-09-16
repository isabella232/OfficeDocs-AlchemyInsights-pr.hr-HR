---
title: Otklanjanje poteškoća s implementacijom certifikata provjere autentičnosti klijenta
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
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658978"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Otklanjanje poteškoća s implementacijom certifikata provjere autentičnosti klijenta

U kombinaciji s drugim vrstama profila, kao što su WiFi, VPN i e-pošte, profili za klijentske certifikate i PKCS/PFX korisnici obično se koriste u vezi s drugim oblicima na servisu Wi Kada su te vrste profila povezane s profilom klijentskog certifikata, ovise o uspješnoj implementaciji tog profila.

Početno postavljanje infrastrukture i povezana konfiguracija profila klijentskog certifikata često je potrebno otklanjanje poteškoća. Detaljne upute za uspješan postavljanje programa NDES Connector i uputa za otklanjanje poteškoća radi izoliranje problema s implementacijom certifikata potražite u članku: 

- [Konfiguriranje infrastrukture radi podrške za SCEP uz Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Pregled radi otklanjanja poteškoća s profilima certifikata u programu Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Pomoću referentne skripte za PowerShell možete provjeriti konfiguraciju. Dodatne informacije potražite u članku umetanje [skripti za provjeru povezivanja certifikata](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Ostali česti problemi**

**Kada pokušam instalirati konektor certifikata na poslužitelj NDES Connector, dobivam poruku: "lozinka u zahtjevu za certifikatom nije moguće provjeriti. Možda je već korišten. Nabavite novu lozinku koju ćete poslati ovim zahtjevom. "**  

Ova poruka znači da morate pokrenuti instalaciju poveznika certifikata kao administratora.

U nekim okruženjima poslužitelji na kojima se izvršava dodatak certifikata moraju koristiti proxy poslužitelj da bi se povezali s Intune, pa povezivanje s certifikatom mora koristiti proxy. U nekim okolnostima NDES konektor ignorira konfigurirane postavke proxyja i možda će biti potrebno konfigurirati postavke proxyja tijekom izvođenja u sigurnosnom kontekstu LocalSystem. 
 
Rješenje je pokretanje preglednika Internet Explorer kao sustava i konfiguriranje proxyja u programu IE. Nakon ponovnog pokretanja servisa Intune Connector, NDES konektor povezuje se s Intune.

**Korisnički uređaji više ne dobivaju certifikate za SCEP iz NDES-a.**

Moguće je da je certifikat za provjeru autentičnosti klijenta izdan na poslužitelju NDES, a naveden tijekom instalacije NDES konektora istekao ili nedostaje. Da biste riješili sljedeće: 
 
1. Deinstalirajte NDES konektor.  
2. Koristite ove pojedinosti da biste zatražili novu provjeru autentičnosti klijenta ili certifikat za provjeru autentičnosti poslužitelja: 
 
    - Naziv predmeta: CN = vanjski FQDN  
    - Zamjenski naziv predmeta (oba su obavezna): DNS = vanjski FQDN, DNS = Internal FQDN 
 
3. Ponovno instalirajte NDES konektor s novim certifikatom.