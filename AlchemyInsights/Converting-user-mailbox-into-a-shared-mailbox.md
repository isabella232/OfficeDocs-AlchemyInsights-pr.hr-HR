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
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496391"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Zajednički poštanski sandučić pretvoriti okvir pošte korisnika

Korisnički poštanski sandučić možete pretvoriti u zajednički poštanski sandučić samo ako korisnik ima Exchange licence. Nakon pretvaranja u poštanskom sandučiću, će nastaviti prikazivati na popisu aktivnih korisnika jer taj popis uključuje zajednički poštanski sandučići. Međutim, pretvorene poštanski sandučić također će prikazati u popisu zajednički poštanski sandučić. 
  
Ako pokušate pretvoriti poštanskog sandučića u Exchange administratorske konzole i pretvorba ne uspije, očistite predmemoriju preglednika i kolačiće i pokušajte ponovno. Ako ga i dalje ne radi, pokušajte pretvoriti u poštanski sandučić Exchange ljuske za upravljanje pokretanjem sljedeće naredbe:
  
```
Set-Mailbox -Type Shared
```

Dodatne informacije o pretvorbi poštanski sandučić je dostupna u [pretvoriti korisnički poštanski sandučić zajednički poštanski sandučić](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
