---
title: Postavljanje DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645664"
---
# <a name="setup-dkim"></a>Postavljanje DKIM

Potpune upute za konfiguriranje DKIM-a za prilagođene domene u sustavu Microsoft 365 [su ovdje](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Za **svaku** prilagođenu domenu morate stvoriti **dva** DKIM CNAME zapisa na servisu za hostiranje DNS-a vaše domene (obično registraru domene). Na primjer, contoso.com i fourthcoffee.com zahtijevaju četiri DKIM CNAME zapisa: dva za contoso.com i dva za fourthcoffee.com.

   DKIM CNAME zapisi za **svaku** prilagođenu domenu koriste sljedeće oblike:

   - **Ime glavnog računala**:`selector1._domainkey.<CustomDomain>`

     **Točke na adresu ili vrijednost:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ime glavnog računala**:`selector2._domainkey.<CustomDomain>`

     **Točke na adresu ili vrijednost:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je tekst s `.mail.protection.outlook.com` lijeve strane u prilagođenom MX zapisu `contoso-com` za prilagođenu domenu (na primjer, za contoso.com domene). \<InitialDomain\> je domena koju ste koristili kada ste se prijavili za Microsoft 365 (na primjer, contoso.onmicrosoft.com).

2. Nakon što stvorite CNAME zapise za prilagođene domene, izvršite sljedeće upute:

   A. [prijavite se u Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomoću računa tvrtke ili obrazovne ustanove.

   B. Odaberite ikonu pokretača aplikacija u gornjem lijevom kutu i odaberite **Administrator**.

   C. U navigaciji u donjem lijevom kutu **proširite Administrator** i odaberite **Exchange**.

   D. Idite na **Zaštita** > **DKIM**.

   E. Odaberite domenu , a zatim odaberite **Omogući** za **potpisivanje poruka za ovu domenu s DKIM potpisima**. Ponovite ovaj korak za svaku prilagođenu domenu.
