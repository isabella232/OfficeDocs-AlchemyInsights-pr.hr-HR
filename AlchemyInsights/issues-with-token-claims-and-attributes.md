---
title: Problemi s potraživanjima i atributima tokena
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012876"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemi s potraživanjima i atributima tokena

**Ažuriranje, konfiguriranje i uklanjanje potraživanja tokena**

1. Pomoću Azure Active Directory (Azure AD) možete [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) prilagoditi vrstu zahtjeva za potraživanje uloga u tokenu za odgovor koji primite nakon autorizacije aplikacije.
2. Razvojni inženjeri aplikacija mogu koristiti neobavezne zahtjeve u aplikacijama Azure AD da bi odredili koje tvrdnje žele u tokenima poslanima u njihovu aplikaciju. Dodatne informacije potražite u članku [Navedite neobavezne zahtjeve za aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Konfiguriranje grupnih zahtjeva za aplikacije Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Ako u aplikaciji koristite besprijekornu jedinstvenu prijavu, pogledajte prilagodba potraživanja izdanih u [SAML tokenu za korporacijske aplikacije](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Mapiranje atributa potraživanja**

1. Da biste konfigurirali pravilnik mapiranja potraživanja pomoću komponente PowerShell, pogledajte prilagodba potraživanja emitiranih u tokenima za određenu [aplikaciju u klijentu (pretpregled).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Atributi proširenja sheme direktorija omogućuju pohranu dodatnih podataka u Azure Active Directory korisničkim objektima i drugim objektima direktorija kao što su grupe, detalji o klijentu, upravitelji servisa. Samo atributi proširenja na korisničkim objektima mogu se koristiti za emitiranje zahtjeva aplikacijama. [Korištenje atributa proširenja sheme direktorija u](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) tvrdnjama opisuje kako koristiti atribute proširenja sheme direktorija za slanje korisničkih podataka aplikacijama u zahtjevima za tokene.

Dodatne informacije o potraživanjima tokena potražite u članku:

- [Potraživanja u pristupne tokene](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Potraživanja u id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Tvrdnje koje](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) možete očekivati u id tokenima i pristupnim tokenima koje izdaje Azure AD B2C
- [Referenca na potraživanja saml tokena](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
