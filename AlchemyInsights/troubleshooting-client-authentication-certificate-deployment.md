---
title: Otklanjanje poteškoća s implementacijom certifikata za provjeru autentičnosti klijenta
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554787"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Otklanjanje poteškoća s implementacijom certifikata za provjeru autentičnosti klijenta

Intune NDES/SCEP i PKCS/PFX Klijentski certifikati profili se obično koriste u kombinaciji s drugim vrstama profila kao što su WiFi, VPN i e-pošta kako bi se korisnicima omogućilo provjeru autentičnosti korporativnih resursa. Kada su te vrste profila povezane s profilom certifikata klijenta ovise o uspješnoj implementaciji tog profila.

Početno postavljanje infrastrukture i pridružena konfiguracija profila klijentske potvrde često zahtijevaju otklanjanje poteškoća. Detaljni vodič za uspješno postavljanje NDES priključka i upute za otklanjanje poteškoća za izoliranje problema s implementacijom certifikata potražite u članku: 

- [Konfiguriranje infrastrukture za podršku SKEP-a s Intuneom](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Pregled otklanjanja poteškoća s profilima certifikata SCEP-a pomoću programa Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Pomoću referencišenih skripti ljuske powershell provjerite konfiguraciju. Dodatne informacije [potražite u odjeljku Skripte za provjeru poveznika certifikata intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Ostala uobičajena pitanja**

**Našto JA pokušati uvesti koga u službu Intune izdati svjedodžbu povezivanje na NDES povezivanje poslužitelj, JA dobiti poruka, " lozinka in izdati svjedodžbu molba ne moći biti verified. Možda je već korišten. Nabavite novu lozinku za slanje s ovim zahtjevom."**  

Ova poruka znači da morate pokrenuti instalaciju poveznika certifikata kao administrator.

U nekim okruženjima poslužitelji na kojima se izvodi Intune certifikat moraju koristiti proxy poslužitelj za povezivanje s intuneom pa poveznik certifikata mora koristiti proxy. U nekim okolnostima NDES Connector zanemaruje konfigurirane postavke proxy poslužitelja i možda će biti potrebno konfigurirati postavke proxy poslužitelja tijekom pokretanja u sigurnosnom kontekstu LocalSystema. 
 
rješenje će biti trčanje Internet explorer kao SISTEM i konfiguracijski proksiji in IE. Nakon ponovnog pokretanja servisa Intune Connector, NDES priključak povezuje se s intune.

**Korisnički uređaji više ne primaju SCEP certifikate iz NDES-a.**

Moguće je da je certifikat za provjeru autentičnosti klijenta izdan ndes poslužitelju i naveden tijekom instalacije NDES priključka istekao ili nedostaje. Da biste riješili problem: 
 
1. Deinstalirajte NDES poveznik.  
2. Koristite ove pojedinosti da biste zatražili novu provjeru autentičnosti klijenta ili certifikat za provjeru autentičnosti poslužitelja: 
 
    - Naziv predmeta: CN=vanjski fqdn  
    - Alternativni naziv predmeta (oba su obavezna): DNS=vanjski fqdn, DNS=interni fqdn 
 
3. Ponovno instalirajte NDES priključak s novim certifikatom.