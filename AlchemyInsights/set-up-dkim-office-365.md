---
title: Postavljanje DKIM u sustavu Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764923"
---
# <a name="setup-dkim-in-office-365"></a>Postavljanje DKIM u sustavu Office 365

Dovršeno upute za konfiguriranje DKIM za prilagođenih domena u sustavu Office 365 su [ovdje](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Za **svaku** prilagođenu domenu, morate stvoriti **dva** DKIM CNAME zapise na vaše domene DNS pružatelju usluge (obično Registrator domene). Ako, na primjer, contoso.com i fourthcoffee.com zahtijevaju četiri zapisa DKIM CNAME: dva za contoso.com i dva za fourthcoffee.com.

   DKIM CNAME zapisa za **svaku** prilagođenu domenu koristite sljedeće formate:

   - **Naziv glavnog računala**:`selector1._domainkey.<CustomDomain>`

     **Točke adresu ili vrijednost**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Naziv glavnog računala**:`selector2._domainkey.<CustomDomain>`

     **Točke adresu ili vrijednost**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je tekst lijevo od `.mail.protection.outlook.com` u prilagođene MX zapisa za prilagođene domene (na primjer, `contoso-com` za contoso.com domene). \<InitialDomain\> je domene koji ste koristili kada ste se prijavili za Office 365 (na primjer, contoso.onmicrosoft.com).

2. Nakon što ste stvorili zapise CNAME za prilagođene domene, dovršite sljedeće upute:

   na. [Prijavite se u Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) s računom poslu ili u školi.

   b. Odaberite ikonu pokretača app u gornju lijevu i odaberite **Admin**.

   c. U donjem lijevom navigacijskom proširite **Admin** i odaberite **Exchange**.

   d. Idi na **zaštitu** > **DKIM**.

   e. Odaberite domenu, a zatim odaberite **Omogući** za **potpisivanje poruke za ovu domenu s potpisima DKIM**. Ponovite ovaj korak za svaku prilagođenu domenu.
