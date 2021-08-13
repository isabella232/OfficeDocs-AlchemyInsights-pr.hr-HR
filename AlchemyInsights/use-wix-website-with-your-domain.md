---
title: Korištenje web-mjesta Wix s Office 365 kupljenim ili upravljanim domenama
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
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980169"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Korištenje web-mjesta Wix s Office 365 kupljenim ili upravljanim domenama

- [Ažuriranje DNS zapisa da biste web-mjesto održavali kod trenutnog davatelja usluge hostiranja](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Članak Wix "Povezivanje domene s Wix-om pomoću načina usmjerivanja" preporučuje korištenje točke (dodavanje DNS zapisa po gornjoj vezi) umjesto promjene poslužitelja naziva prilikom korištenja Office 365
- Ako i dalje želite promijeniti poslužitelje naziva u Wix, morat ćete stvoriti DNS zapise na servisu  [Wix za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Ako je vaša domena kupljena od Microsofta, nazivne poslužitelje nije moguće promijeniti. Ako morate promijeniti poslužitelje naziva, Microsoftova kupljena domena mora se prenijeti drugom  [davatelju usluge hostiranja nakon 60 dana](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)