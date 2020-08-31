---
title: Korištenje Wix web-mjesta sa sustavom Office 365 kupljene i upravljanih domena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300690"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Korištenje Wix web-mjesta sa sustavom Office 365 kupljene i upravljanih domena

- [Ažuriranje DNS zapisa radi zadržavanja web-mjesta s trenutnim davatelja usluga hostiranja](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix članak "povezivanje domene sa sustavom Wix pomoću metode pokazujući" preporučuje se pomoću pokazivačkog upućivanjem (Dodavanje DNS zapisa na gornju vezu), a ne promjenom poslužitelja naziva prilikom korištenja sustava Office 365
- Ako i dalje odaberete promjenu naziva poslužitelja u Wix, morat ćete  [stvoriti DNS zapise u programu Wix za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Ako je vaša domena kupljena od Microsofta, poslužitelji naziva ne mogu se promijeniti. Ako morate promijeniti poslužitelje naziva, Microsoftova kupljena domena trebala bi se [prenijeti na drugog davatelja usluge hostiranja nakon 60 dana](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host) .