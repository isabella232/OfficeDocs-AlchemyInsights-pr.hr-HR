---
title: Pretvaranje korisnički poštanski sandučić u zajednički poštanski sandučić?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28280630"
---
Korisnički poštanski sandučić možete pretvoriti u zajednički poštanski sandučić samo ako korisnik ima Exchange licence. Nakon pretvaranja u poštanskom sandučiću, će nastaviti prikazivati na popisu aktivnih korisnika jer taj popis uključuje zajednički poštanski sandučići. Međutim, pretvorene poštanski sandučić također će prikazati u popisu zajednički poštanski sandučić. 
  
Ako pokušate pretvoriti poštanskog sandučića u Exchange administratorske konzole i pretvorba ne uspije, očistite predmemoriju preglednika i kolačiće i pokušajte ponovno. Ako ga i dalje ne radi, pokušajte pretvoriti u poštanski sandučić Exchange ljuske za upravljanje pokretanjem sljedeće naredbe:
  
```
Set-Mailbox -Type Shared
```

Dodatne informacije o pretvorbi poštanski sandučić je dostupna u [pretvoriti korisnički poštanski sandučić zajednički poštanski sandučić](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
