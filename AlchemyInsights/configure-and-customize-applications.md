---
title: Konfiguriranje i prilagodba aplikacija
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044980"
---
# <a name="configure-and-customize-applications"></a>Konfiguriranje i prilagodba aplikacija

**Konfiguriranje aplikacija**

1. [Brzi početak rada: konfiguriranje svojstava za aplikaciju u klijentu servisa Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) pokazuje kako konfigurirati neka svojstva aplikacije.
2. Da bismo vam pomogli integrirati aplikacije Azure Active Directory, razvili smo zbirku [vodiča koji](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) će vas kroz konfiguraciju.
3. [Konfiguriranje aplikacije Proxy aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) omogućuje vam da shvatite kako konfigurirati aplikaciju proxy aplikacije na servisu Azure AD da biste lokalne aplikacije izložili oblaku.
4. [Preuzmite PingAccess i](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)konfigurirajte aplikaciju: Slijedite upute u web-mjestu Konfiguriranje *značajke PingAccess* za Azure AD da biste zaštitili aplikacije objavljene pomoću proxyja aplikacije Microsoft Azure AD na web-mjestu Identitet pinga i preuzmite najnoviju verziju značajke PingAccess.

**Pogreške u pogrešno konfiguriranoj aplikaciji (AADSTS650056)**

1. Provjerite pristupate li aplikaciji s adrese za prijavu koju vam je pružio vlasnik aplikacije. U suprotnom se pomoću uobičajenog postupka prijavite u aplikaciju. U većini slučajeva to će se automatski riješiti prirodno. Ako se ne riješi, ova objava može pomoći u otklanjanju poteškoća i rješavanju tog problema.
2. **Ako je vaša tvrtka ili ustanova vlasnik aplikacije** (što znači da je registracija aplikacije u vašoj tvrtki ili ustanovi):
    - Barem preporučujemo da se doda `User.Read` dozvola tvrtke Microsoft `openid` **Graph** ovlaštenih korisnika.
    - Provjerite jesu li aplikacija i sve njegove dozvole privučene. To možete provjeriti tako  da u odjeljku Dozvole API-ja potražite stupac Status **registracije aplikacije**.
    - U nekim scenarijima aplikacija može biti treća strana, no možda je registrirana u vašoj tvrtki ili ustanovi. Provjerite je li ta aplikacija navedena u registracijama aplikacije (nije Enterprise aplikacija).
    - Ako vam se i dalje prikazuje ova poruka o pogrešci. Potom ćete možda morati izraditi URL pristanka opisan u **4. koraku**.
3. **Ako vaša tvrtka ili ustanova nije vlasnik aplikacije i koristi je kao aplikaciju drugih proizvođača:**
    - Ako ste administrator za globalnu tvrtku/tvrtku, trebali biste vidjeti zaslon za pristanak. Potvrdite okvir za **"Pristanak u ime tvrtke ili ustanove".**
    - Ako ne vidite zaslon za pristanak, izbrišite aplikaciju Enterprise i pokušajte ponovno.
    - Ako vam se i dalje prikazuje ova poruka o pogrešci. Potom ćete možda morati izraditi URL pristanka opisan u **4. koraku**.
4. **Ručno izradite URL** pristanka koji će se koristiti: ako je aplikacija osmišljena za pristup određenom resursu, možda nećete moći koristiti gumbe pristanak s portala Azure, morat ćete ručno generirati VLASTITI URL pristanka i koristiti ga.
    - Morat ćete nabaviti i `{App-Id}` vlasnika `{App-Uri-Id}` aplikacije. `{Tenant-Id}` bit će vaš identifikator klijenta. To će biti ili `yourdomain.onmicrosoft.com` VAŠ ID direktorija.
    - Ako se aplikacija sama pristupa resursu, ona `{App-Id}` će `{App-Uri-Id}` biti ista.
5. Dodatne informacije potražite u članku Problemi prilikom prijave u konfigurirane aplikacije za jedinstvenu prijavu utemeljenu [na SAML-u](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Prilagodba aplikacija**

- [Dodajte brendiranje na](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) stranicu za prijavu u Azure Active Directory tvrtke ili ustanove – pomoću logotipa tvrtke ili ustanove i prilagođenih shema boja na stranicama za prijavu na Azure Active Directory (Azure AD).
- [Dodajte prilagođeni naziv domene pomoću portala Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – svaki novi klijent servisa Azure AD isporučuje se s početnim nazivom domene. Ne možete promijeniti ni izbrisati početni naziv domene, ali možete dodati nazive tvrtke ili ustanove. Dodavanje prilagođenih naziva domena olakšava stvaranje korisničkih imena koja su poznata vašim korisnicima.
