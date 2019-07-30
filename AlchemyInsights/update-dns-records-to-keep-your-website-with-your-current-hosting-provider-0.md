---
title: Ažuriranje zapisa DNS zadržati svoje web-mjesto s trenutnom pružatelju usluge
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: e437015d476c1417fa37e1b1c250e2205e9ce4d9
ms.sourcegitcommit: b825ced7b66d452b0f3874a57e033e690ec41c93
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/29/2019
ms.locfileid: "35925277"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Ažuriranje zapisa DNS zadržati svoje web-mjesto s trenutnom pružatelju usluge

1. Na stranici [domena](https://portal.office.com/adminportal/home#/Domains) popisa domena, odaberite domenu koju koristite za vaše web-mjesto.

2. Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:

  - **Vrsta DNS** unesite: **(adresa)**

  - Za **naziv glavnog računala ili pseudonim**, upišite sljedeće:**@**

  - Za **IP adresu**, upišite statičku IP adresu za vaše web-mjesto gdje ga trenutno hostuje (na primjer, 172.16.140.1).

    To mora biti *statička* IP adresa za web-mjesto, ne *dinamičku* IP adresu. Provjerite s gdje je smještena vaše web-mjesto za dobivanje statičku IP adresu za vaše javne web-mjesta.

3. Odaberite **Spremi**.

Osim toga, možete stvoriti zapis CNAME pomoći klijentima da pronađu vaše web-mjesto.
  
1. Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:

  - **Vrsta DNS** unesite: **CNAME (pseudonima)**

  - Za **naziv glavnog računala ili pseudonim**, upišite sljedeće: **www**

  - **Točke adresu**, upišite je potpuno kvalificirani naziv domene (FQDN) za web-mjesto (na primjer, contoso.com).

2. Odaberite **Spremi**.
