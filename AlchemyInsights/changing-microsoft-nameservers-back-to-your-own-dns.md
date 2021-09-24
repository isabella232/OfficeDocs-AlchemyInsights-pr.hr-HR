---
title: Povratak s Microsoftovih poslužitelja naziva na upravljanje vlastitim DNS zapisima
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506280"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Povratak s Microsoftovih poslužitelja naziva na upravljanje vlastitim DNS zapisima

Prethodno ste promijenili NS zapise tako da upućite na Microsoft (ns1.bdm.microsoftonline.com), ali ste odlučili upravljati vlastitim DNS zapisima:

Na web-mjestu registrara domene vratite poslužitelj naziva u registrar ili prethodnu postavku. Ako niste upoznati s DNS-om, obratite se podršci kod registrara domena. Imajte na umu da prijenos promjena poslužitelja naziva može potrajati i do 48 sati. 

1. Na portalu Microsoft 365 administratora idite **na Postavke** Domene , potvrdite okvir uz domenu pa  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)odaberite **Upravljanje DNS-om**. 

2. U čarobnjaku odaberite **Dodaj vlastite DNS zapise i** dovršite čarobnjak. Time se mijenja način upravljanja DNS-om, a zatim omogućuje dodavanje prilagođenih DNS zapisa potrebnih za podršku odabranim servisima.

Ako ste zapise poslužitelja naziva promijenili u Microsoft i imate web-mjesto, možete dodati DNS zapise za web-mjesto umjesto da ponovno promijenite poslužitelje naziva. Dodatne informacije potražite u članku Ažuriranje DNS zapisa da [biste web-mjesto održavali kod trenutnog davatelja usluge hostiranja.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


