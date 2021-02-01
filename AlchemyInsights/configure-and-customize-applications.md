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
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063593"
---
# <a name="configure-and-customize-applications"></a>Konfiguriranje i prilagodba aplikacija

**Konfiguriranje aplikacija**

1. [Brzo pokretanje: Konfiguriranje svojstava aplikacije u klijentu Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) prikazuje kako konfigurirati neke od svojstava za aplikaciju.
2. Da biste integrirali aplikacije s servisom Azure Active Directory, razvili smo [zbirku tutoriali](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) koji vas prolaze kroz konfiguraciju.
3. [Kako konfigurirati aplikaciju proxyja aplikacija](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) olakšava vam da razumijete kako konfigurirati aplikaciju proxyja aplikacije u sklopu servisa Azure ad da biste u oblak izložili lokalne aplikacije.
4. [Preuzmite pingaccess i konfigurirajte aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): slijedite upute u *odjeljku Konfigurirajte Pingaccess za Azure ad da biste zaštitili aplikacije* objavljene pomoću proxy poslužitelja aplikacije Microsoft Azure ad na web-mjestu ping Identity i preuzeli najnoviju verziju programa pingaccess.

**Pogrešno konfigurirane aplikacije (AADSTS650056) pogreške**

1. Pobrinite se da pristupate aplikaciji putem adrese za prijavu koju vam je dao vlasnik aplikacije. U suprotnom smislu, prijavite se u aplikaciju putem normalnog postupka. U većini slučajeva to će se naravno automatski riješiti. Ako to ne učinite, ovaj post može olakšati otklanjanje poteškoća i njihovo rješavanje.
2. **Ako je vaša tvrtka ili ustanova vlasnik aplikacije** (što znači da je registracija aplikacija u vašoj tvrtki ili ustanovi):
    - U najmanju ruku preporučamo da se `User.Read` doda ili `openid` delegirana dozvola iz **programa Microsoft Graph** .
    - Provjerite jesu li aplikacija i sve njezine dozvole suglasne. To možete provjeriti tako da pogledate stupac **status** registracije prijave u sklopu **API dozvola**.
    - U nekim scenarijima aplikacija može biti treća strana, no možda je registrirana u vašoj tvrtki ili ustanovi. Potvrdite je li ova aplikacija navedena u registracijama aplikacija (ne u korporacijskim aplikacijama).
    - Ako se poruka o pogrešci i dalje prikazuje. Onda ćete možda morati stvoriti URL pristanka opisan u četvrtom **koraku**.
3. **Ako vaša tvrtka ili ustanova nije vlasnik aplikacije te ga koristi kao aplikaciju drugih proizvođača**, učinite sljedeće:
    - Ako ste administrator globalne/tvrtke, trebali biste vidjeti zaslon pristanka. Provjerite jeste li potvrdili okvir za **"pristanak u ime tvrtke ili ustanove"**.
    - Ako ne vidite zaslon pristanka, izbrišite Enterprise aplikaciju, a zatim pokušajte ponovno.
    - Ako se poruka o pogrešci i dalje prikazuje. Onda ćete možda morati stvoriti URL pristanka opisan u četvrtom **koraku**.
4. **Ručno stvaranje URL-a pristanka koji** će se koristiti: ako je aplikacija dizajnirana za pristup određenom resursu, možda nećete moći koristiti gumbe za pristanak na portalu Azure, morat ćete ručno GENERIRATI vlastiti URL pristanka i koristiti ovo.
    - Morat ćete dobiti `{App-Id}` i `{App-Uri-Id}` od vlasnika aplikacije. `{Tenant-Id}` Bit će vaš identifikator korisnika. To će biti `yourdomain.onmicrosoft.com` ili ID imenika.
    - Ako se aplikacijom omogućuje pristup resursu, onda će `{App-Id}` i ona `{App-Uri-Id}` biti ista.
5. Dodatne informacije potražite u članku [problemi prilikom prijave na pojedinačne aplikacije koje se temelje na jednom](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)servisu.

**Prilagodba aplikacija**

- [Dodajte branding na stranicu za prijavu na Azure Active Directory u tvrtki ili ustanovi](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) – koristite logotip tvrtke ili ustanove i prilagođene sheme boja da biste omogućili dosljedan izgled i dojam na stranice za prijavu u Azure Active Directory (Azure AD).
- [Dodajte prilagođeni naziv domene pomoću portala Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – svaki novi stanar Azure ad isporučuje se s početnim nazivom domene. Ne možete promijeniti ili izbrisati početni naziv domene, ali možete dodati nazive tvrtke ili ustanove. Dodavanje prilagođenih naziva domena olakšava stvaranje korisničkih imena koja su poznata korisnicima.
