---
title: Problemi s vezama i URL-ovima
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974227"
---
# <a name="issues-with-links-and-urls"></a>Problemi s vezama i URL-ovima

Preusmjeravanje URI-a/URL-ova za odgovaranje (oba izraza su zamjenjivi) URL-ovi koje koristi Microsoftova platforma identiteta radi povratka žetona zatraženih od aplikacije. Informacije o tim URL adresama potražite u sljedećim člancima:

- [Protoci provjere autentičnosti i scenariji aplikacija](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informacije o preusmjeravanju Uris-a na stranici **Registracija aplikacija** za svaki scenarij.
- [Ograničenja i ograničenja za preusmjeravanje URI-ja/odgovora](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Ne znam kako registrirati upute za preusmjeravanje u programu URI/Reply za moju aplikaciju**

Kada se prijavite pomoću aplikacije koju razvijate, ako dijaloški okvir za prijavu prikazuje **AADSTS50011: URL za odgovor naveden u zahtjevu ne podudara se s URL-ovima za odgovaranje koji su konfigurirani za <your app ID> aplikaciju**, morat ćete dodati u registraciju aplikacija, Uri preusmjeravanja koji je vaš kod korišten u zahtjevu tokena na Microsoftovu platformu identiteta.

Da biste dodali URL za odgovor, otvorite karticu **Provjera autentičnosti** na stranici **Registracija aplikacija** na portalu Azure i dodajte unos u odjeljak **preusmjeravanje Uris** -a. Preusmjereni su URIs (web ili mobilni/stolna računala). Vrijednost koju morate unijeti ovisi o vrsti aplikacije koju sastavljate, kao što je opisano u nastavku:

- Za aplikacije za jednu stranicu i web-aplikacije, URL za odgovor jest URL u aplikaciji. Pogledajte [registraciju aplikacija za jednu stranicu](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ili [Registriranje aplikacije web-aplikacije pomoću portala Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Vrijednost koju morate odabrati ovisi o aplikacijama za stolna računala:
    - platforma (MacOS se razlikuje od sustava Windows ili Linuxa)
    - način dobivanja tokena (interaktivno, s protočnim kodom uređaja, uz integriranu provjeru autentičnosti sustava Windows [IWA] ili uz korisničko ime/lozinku).
    Pojedinosti potražite u članku [aplikacije za stolna računala – registracija aplikacija – URi za preusmjeravanje](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Za mobilne aplikacije, URI preusmjeravanja ovisi o:
    - platforma (iOS/Android/UWP)
    - informacije koje se koriste za izgradnju aplikacije, kao što je ID paketa u sustavu iOS, te popis proizvoda i raspršivanje potpisa na servisu Android, registracija aplikacija Azure portal pomoći će vam. Pojedinosti potražite u članku [Konfiguracija platforme i preusmjeravanje URIs-a](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Web-API-jevi i neki tihi načini stjecanja tokena (IWA i username/lozinka) ne zahtijevaju URI za preusmjeravanje.

**Rasporedio sam web-aplikaciju i kada testiram aplikaciju za razmještene poruke, dobivam nepodudarnost URL-a za odgovor**

Dodajte preusmjeravanje URIs-a za sva mjesta na kojima implementirate web-aplikaciju. Dodatne informacije potražite u članku [Registriranje aplikacije web-aplikacije pomoću portala Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Dodajte URI preusmjeravanja na mjesto odmah nakon implementacije aplikacije na tom mjestu.

**Ne mogu registrirati dovoljno URL-ova za odgovaranje**

Vi ste ISV i imate jedan ili više preusmjeravanja URIs-a za svakog klijenta. Želite migrirati iz servisa ADAL/Azure AD v 1,0 na MSAL/Microsoftovu platformu za identitete i možete pritisnuti [maksimalan broj preusmjeravanja URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)-a. Da biste riješili taj problem, [Dodajte preusmjeravanje URIs-a u ravnatelje servisa](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) koji odgovaraju svakom od vaših kupaca.
