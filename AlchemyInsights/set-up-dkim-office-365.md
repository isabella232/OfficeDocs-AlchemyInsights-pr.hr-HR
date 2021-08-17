---
title: Postavljanje DKIM-a
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108548"
---
# <a name="setup-dkim"></a>Postavljanje DKIM-a

Cjelovite upute za konfiguriranje DKIM-a za prilagođene domene u aplikaciji Microsoft 365 su [ovdje](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Za **svaku** prilagođenu domenu morate stvoriti **dva** DKIM CNAME zapisa na servisu za hostiranje DNS-a domene (obično registrar domene). Primjerice, contoso.com fourthcoffee.com četiri DKIM CNAME zapisa: dva za contoso.com i dva za fourthcoffee.com.

   DKIM CNAME zapisi za **svaku prilagođenu** domenu koriste sljedeće oblike:

   - **Naziv glavnog računala:**`selector1._domainkey.<CustomDomain>`

     **Upućuje na adresu ili vrijednost:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Naziv glavnog računala:**`selector2._domainkey.<CustomDomain>`

     **Upućuje na adresu ili vrijednost:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je tekst s lijeve strane u prilagođenom `.mail.protection.outlook.com` MX zapisu za prilagođenu domenu (na primjer, `contoso-com` za domenu contoso.com). \<InitialDomain\>je domena koju ste koristili prilikom registracije za Microsoft 365 (npr. contoso.onmicrosoft.com).

2. Kada izradite CNAME zapise za prilagođene domene, slijedite sljedeće upute:

   a. [prijavite se u Microsoft 365 pomoću](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) računa za posao ili školu.

   b. Odaberite ikonu pokretača aplikacija u gornjem lijevom kutu i odaberite **Administrator**.

   c. U donjem lijevom navigacijskom oknu **proširite Odjeljak Administrator** i **odaberite Exchange**.

   d. Idite **na Zaštita**  >  **DKIM**.

   e. Odaberite domenu, a zatim **odaberite Omogući** **za potpisivanje poruka za ovu domenu s DKIM potpisima**. Ponovite ovaj korak za svaku prilagođenu domenu.
