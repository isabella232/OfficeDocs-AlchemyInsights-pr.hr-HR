---
title: Pretvaranje korisnički poštanski sandučić u zajednički poštanski sandučić?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374315"
---
Korisnički poštanski sandučić možete pretvoriti u zajednički poštanski sandučić samo ako korisnik ima Exchange licence. Nakon pretvaranja u poštanskom sandučiću, će nastaviti prikazivati na popisu aktivnih korisnika jer taj popis uključuje zajednički poštanski sandučići. Međutim, pretvorene poštanski sandučić također će prikazati u popisu zajednički poštanski sandučić. 
  
Ako pokušate pretvoriti poštanskog sandučića u Exchange administratorske konzole i pretvorba ne uspije, očistite predmemoriju preglednika i kolačiće i pokušajte ponovno. Ako ga i dalje ne radi, pokušajte pretvoriti u poštanski sandučić Exchange ljuske za upravljanje pokretanjem sljedeće naredbe:
  
```
Set-Mailbox -Type Shared
```

Dodatne informacije o pretvorbi poštanski sandučić je dostupna u [pretvoriti korisnički poštanski sandučić zajednički poštanski sandučić](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
