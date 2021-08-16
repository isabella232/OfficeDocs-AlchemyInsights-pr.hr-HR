---
title: Problemi s vezama i URL-ovima
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054790"
---
# <a name="issues-with-links-and-urls"></a>Problemi s vezama i URL-ovima

URI za preusmjeravanje/URL-ovi za odgovore (oba su izraza zamjenjiva) su URL-ovi koje Microsoftova platforma za identitete upotrebljava za vraćanje tokena koje su zatražile aplikacije. Dodatne informacije o ovim URL-ovima potražite u sljedećim člancima:

- [Tijekovi provjere autentičnosti i scenariji aplikacije](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informacija o URI-jima za preusmjeravanje u **stranici za** registraciju aplikacije za svaki scenarij.
- [Ograničenja URI-ja za preusmjeravanje/URL-a za odgovore ](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Ne znam kako registrirati pravi URI za preusmjeravanje / URL za odgovore za moju aplikaciju**

Kad se prijavite s aplikacijom koju razvijate, ako dijaloški okvir za prijavu prikazuje **AADSTS50011: url specificiran u zahtjevu ne podudara se s url-ovima za odgovore konfigurirane za aplikaciju <your app ID>**,svojoj registraciji aplikacije morat ćete dodati URL za preusmjeravanje koji je vaš kod upotrijebio u zahtjevu za token na Microsoftovu platformu identiteta.

Za dodavanje URL-a za odgovore idite na karticu **Provjera autentičnosti** u stranici za registraciju **svoje aplikacije** na Azure portalu i dodajte unos u odjeljak **URI-ji** za preusmjeravanje. Vrijednost koju trebate unijeti ovisi o vrsti aplikacije koju izrađujete, kao što je opisano u nastavku:

- Za aplikacije od jedne stranice i web-aplikacije, URL za odgovore je URL u vašoj aplikaciji,. Pogledajte [registraciju aplikacije od jedne stranice](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ili [registrirajte web-aplikaciju pomoću portala Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Za aplikacije za stolna računala, vrijednost koju trebate odabrati ovisi o:
    - platformi (MacOS je različit od sustava Windows ili Linux)
    - načinu pribavljanja tokena (interaktivno, s tijekom koda uređaja, s integriranom provjerom autentičnosti u sustavu Windows [IWA] ili s korisničkim imenom/lozinkom.
    Za detalje, pogledajte [Aplikacije za stolna računala – registracija aplikacije – URi za preusmjeravanje](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Za mobilne aplikacije, URI za preusmjeravanje ovisi o:
    - platformi (iOS/Android/UWP)
    - podacima koji se upotrebljavaju za izradu vaše aplikacije, kao što su ID paketa u iOS-u te naziv paketa i raspršivanje potpisa na Androidu. Pomoći će vam registracija portala Azure. Za pojedinosti pogledajte [Konfiguracija platforme i URI-jevi za preusmjeravanje](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> API-ji za web i neki od tihih načina za nabavljanje tokena (IWA i korisničko ime/lozinka) ne zahtijevaju URI za preusmjeravanje.

**Implementirao sam web-aplikaciju i kad sam je testirao, dobivam poruku o nepodudaranju url-a za odgovore**

Dodajte URI-je za preusmjeravanje za sve lokacije na kojima implementirate web-aplikaciju. Za dodatne informacije pogledajte [Registrirajte web-aplikaciju pomoću portala Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Dodajte URI za preusmjeravanje za lokaciju odmah nakon što ste implementirali aplikaciju na toj lokaciji.

**Ne mogu registrirati dovoljno URL-ova za odgovore**

Vi ste ISV i imate jedan ili nekoliko URI-ja za preusmjeravanje za svakog svog klijenta. Želite migrirati s ADAL/Azure AD v1.0 na MSAL/Microsoftovu platformu za identitete i pogodili ste [maksimalan broj URL-ova za preusmjeravanje](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Da biste ovo riješili, [dodajte URL-ove za preusmjeravanje na upravitelje servisa](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) koji odgovaraju svakom od vaših korisnika.
