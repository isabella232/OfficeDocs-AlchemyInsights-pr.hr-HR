---
title: Korištenje web-mjesta Wix s kupljenim ili upravljanim domenama sustava Office 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825939"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Korištenje web-mjesta Wix s kupljenim ili upravljanim domenama sustava Office 365

- [Ažuriranje DNS zapisa da biste web-mjesto održavali kod trenutnog davatelja usluge hostiranja](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Članak Wix "Povezivanje domene s Wix-om pomoću načina usmjerivanja" preporučuje korištenje točke (dodavanje DNS zapisa po gornjoj vezi) umjesto promjene poslužitelja naziva prilikom korištenja sustava Office 365
- Ako i dalje želite promijeniti poslužitelje naziva u Wix, morat ćete stvoriti DNS zapise na servisu  [Wix za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Ako je vaša domena kupljena od Microsofta, nazivne poslužitelje nije moguće promijeniti. Ako morate promijeniti poslužitelje naziva, Microsoftova kupljena domena mora se prenijeti drugom  [davatelju usluge hostiranja nakon 60 dana](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)