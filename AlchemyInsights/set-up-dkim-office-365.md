---
title: Postavljanje DKIM-a
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509376"
---
# <a name="setup-dkim"></a>Postavljanje DKIM-a

Ovdje [su](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)potpune upute za konfiguriranje DKIM-a za prilagođene domene u sustavu Microsoft 365 .

1. Za **svaku** prilagođenu domenu morate stvoriti **dva** DKIM CNAME zapisa na servisu za hostiranje DNS-a vaše domene (obično registrar domene). Na primjer, contoso.com i fourthcoffee.com zahtijevaju četiri DKIM CNAME zapisa: dva za contoso.com i dva za fourthcoffee.com.

   DKIM CNAME zapisi za **svaku** prilagođenu domenu koriste sljedeće oblike:

   - **Naziv glavnog računala**:`selector1._domainkey.<CustomDomain>`

     **Upućuje na adresu ili vrijednost:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Naziv glavnog računala**:`selector2._domainkey.<CustomDomain>`

     **Upućuje na adresu ili vrijednost:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>je tekst s lijeve strane `.mail.protection.outlook.com` u prilagođenom MX zapisu za prilagođenu domenu (na primjer, `contoso-com` za domenu contoso.com). \<InitialDomain\>je domena koju ste koristili prilikom registracije za Microsoft 365 (na primjer, contoso.onmicrosoft.com).

2. Nakon što stvorite CNAME zapise za prilagođene domene, dovršite sljedeće upute:

   A. [prijavite se u Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomoću računa tvrtke ili obrazovne ustanove.

   B. Odaberite ikonu pokretača aplikacija u gornjem lijevom kutu i odaberite **Administrator**.

   C. U navigaciji donjeg lijevog lijevog odaberite **Administrator** i odaberite **Exchange**.

   D. Idite na **Zaštita**  >  **DKIM**.

   E. Odaberite domenu, a zatim **odaberite Omogući** za **potpisivanje poruka za ovu domenu pomoću DKIM potpisa**. Ponovite ovaj korak za svaku prilagođenu domenu.
