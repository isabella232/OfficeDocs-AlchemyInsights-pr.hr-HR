---
title: Postavljanje funkcije
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808699"
---
# <a name="setup-dkim"></a>Postavljanje funkcije

U programu Microsoft [365 nalaze se](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)potpune upute za konfiguriranje servisa d ' dekima za prilagođene domene u Microsoftu.

1. Za **svaku** prilagođenu domenu morate stvoriti **dva** DKIM CNAME zapisa na servisu za hostiranje DNS-a u domeni (obično je registrar domena). Primjerice, contoso.com i fourthcoffee.com zahtijevaju četiri DKIM CNAME zapisa: dva za contoso.com i dva za fourthcoffee.com.

   Zapisi u programu defunkcija CNAME za **svaku** prilagođenu domenu koriste sljedeće oblike:

   - **Naziv glavnog računala**: `selector1._domainkey.<CustomDomain>`

     **Upućuje na adresu ili vrijednost**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Naziv glavnog računala**: `selector2._domainkey.<CustomDomain>`

     **Upućuje na adresu ili vrijednost**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je li tekst s desne strane `.mail.protection.outlook.com` u PRILAGOĐENOM MX zapisu za prilagođenu domenu (na primjer, `contoso-com` za domenu contoso.com). \<InitialDomain\> domena koju ste koristili kada ste se prijavili za Microsoft 365 (na primjer, contoso.onmicrosoft.com).

2. Kada stvorite CNAME zapise za prilagođene domene, ispunite sljedeće upute:

   je. [prijavite se u Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomoću računa tvrtke ili obrazovne ustanove.

   b. U gornjem desnom kutu odaberite ikonu Pokretača aplikacija, a zatim **administrator**.

   c. U donjem desnom navigacijskom oknu proširite **administrator** i odaberite **Exchange**.

   d. Idite na **zaštitu**  >  **d-kim**.

   e. Odaberite domenu, a zatim odaberite **Omogući** za **potpisivanje poruka za ovu domenu s DKIM potpisima**. Ponovite ovaj korak za svaku prilagođenu domenu.
