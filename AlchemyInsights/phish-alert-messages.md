---
title: 2491 Upozorenje poruka e-pošte iz pravila "Krađa identiteta isporučena zbog nadjačavanja klijenta ili korisnika"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758900"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Upozoravajte poruke e-pošte iz pravila "Krađa identiteta isporučena zbog nadjačavanja klijenta ili korisnika"

Zadano pravilo upozorenja pod nazivom "Krađa identiteta isporučena zbog nadjačavanja klijenta ili korisnika" uvedena je na klijentima s atp i P2 licencama za Office 365. Ako ste primili ovo upozorenje, evo koraka za istraživanje:

1. U poruci upozorenja kliknite **Prikaz upozorenja** da biste otišli na stranicu **Upozorenja** u centru za & usklađenosti.

2. Odaberite upozorenje da biste vidjeli mogućnost **Prikaz popisa poruka** ili Prikaz poruka u **exploreru**. Obje ove mogućnosti vode vas do pojedinosti poruke, što uključuje ID poruke. Imajte na umu da će veza Threat Explorer automatski filtrirati poruke koje odgovaraju kriterijima upozorenja. Možda ćete morati prilagoditi filtar datuma u programu Threat Explorer.

Poruka o krađi identiteta isporučena je zbog ručno konfiguriranog nadjačavanja:

- Dopušteni pošiljatelj ili domena koje je postavio korisnik.

- Dopušteni pošiljatelj ili domena koje je administrator postavio u pravilima protiv neželjene pošte.

- Dopuštena IP adresa u pravilniku filtra veze.

- Pravilo tijeka pošte (poznato i kao pravilo prijenosa) konfigurirano tako da dopušta poruke.

Ako smatrate da je poruka pogrešno označena kao krađa identiteta, upotrijebite [dodatak Poruka izvješća programa](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook da biste microsoftu poslali uzorke poruka.
