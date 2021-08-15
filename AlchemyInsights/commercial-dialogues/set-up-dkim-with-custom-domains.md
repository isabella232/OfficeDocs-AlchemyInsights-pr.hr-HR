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
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994785"
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
> [!NOTE]
> **DomainGUID** je tekst lijevo od **.mail.protection.outlook.com** u prilagođenom MX zapisu za prilagođenu domenu (npr. contoso-com za **domenu contoso.com**). **InitialDomain je** domena koju ste koristili prilikom registracije za Office 365 (npr. **contoso.onmicrosoft.com).**

Dodatne informacije o DNS zapisima potražite u članku Stvaranje DNS zapisa kod bilo kojeg [davatelja usluge hostiranja DNS-a za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).