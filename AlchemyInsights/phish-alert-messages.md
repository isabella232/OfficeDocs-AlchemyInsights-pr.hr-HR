---
title: Poruka upozorenja e-pošte 2491 iz pravila Phish isporučiti klijentske ili korisnik nadjačati
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391164"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Poruka upozorenja e-pošte iz pravila Phish isporučiti klijentske ili korisnik nadjačati

Zadano upozorenja pravilo pod nazivom "Phish Delivered zbog nadjačavanje korisnika ili klijentske" ima je poslednjeg samoposlužni s Office 365 ATP P1 i P2 licence. Ako ste primili ovo upozorenje, ovdje se istražiti koraka:

1. Iz poruke upozorenja kliknite **Prikaz upozorenja** da biste otišli na stranicu **upozorenja** u & usklađenosti centar sigurnosti.

2. Odaberite upozorenje da biste vidjeli mogućnost za **Prikaz popisa poruka** ili **Prikaz poruka u programu Explorer**. Obje ove opcije poduzeti za pojedinosti poruke uključuje ID poruke. Imajte na umu vezu prijetnja Explorer automatski filtrirali poruke koje zadovoljavaju kriterije upozorenja. Možda ćete morati prilagoditi filtar datuma u programu Explorer prijetnja.

Phishing poruka isporučena zbog ručno konfiguriran nadjačavanje:

- Dopuštenih pošiljatelja ili domene postavio korisnik.

- Dopuštenih pošiljatelja ili domene postavio admin pravila protiv neželjene pošte.

- Dopuštenih IP adresu u pravilima filtar veze.

- Mail protok pravilo (poznate i kao pravilo prijevoza) koja je konfigurirana za dopuštanje poruka u.

Ako mislite da poruka pogrešno označena kao phish, koristite u Outlook [poruka izvještaja dodatak](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) slanje uzoraka poruku tvrtki Microsoft.
