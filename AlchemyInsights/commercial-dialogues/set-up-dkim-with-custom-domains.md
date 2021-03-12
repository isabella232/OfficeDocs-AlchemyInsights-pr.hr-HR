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
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743531"
---
# <a name="set-up-dkim-with-custom-domains"></a>Postavljanje DKIM-a s prilagođenim domenama

Za svaku prilagođenu domenu u DNS-u morate objaviti dva CNAME zapisa. Da biste to učinili, koristite sljedeći oblik:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **Domainguid** je tekst s desne strane **. mail.Protection.Outlook.com** u prilagođenom MX zapisu za prilagođenu domenu (na primjer, contoso-com za domenu **contoso.com**). **Initialdomena** je domena koju ste koristili prilikom prijave za Office 365 (na primjer, **contoso.onmicrosoft.com**).

Dodatne informacije o DNS zapisima potražite u članku [Stvaranje DNS zapisa kod bilo kojeg davatelja usluge HOSTIRANJA DNS-a za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).