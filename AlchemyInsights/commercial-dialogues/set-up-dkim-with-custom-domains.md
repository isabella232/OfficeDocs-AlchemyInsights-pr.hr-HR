---
title: Postavljanje DKIM-a s prilagođenim domenama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332299"
---
# <a name="set-up-dkim-with-custom-domains"></a>Postavljanje DKIM-a s prilagođenim domenama

Morate objaviti dva CNAME zapisa za svaku prilagođenu domenu u DNS-u. Da biste to učiniti, koristite sljedeći oblik:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Napomena:** **DomainGUID** je tekst lijevo od **.mail.protection.outlook.com** u prilagođenom MX zapisu za prilagođenu domenu (npr. contoso-com za **domenu contoso.com).** **InitialDomain je** domena koju ste koristili prilikom registracije za Office 365 (npr. **contoso.onmicrosoft.com).**

Dodatne informacije o DNS zapisima potražite u članku Stvaranje DNS zapisa kod bilo kojeg [davatelja usluge hostiranja DNS-a za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).