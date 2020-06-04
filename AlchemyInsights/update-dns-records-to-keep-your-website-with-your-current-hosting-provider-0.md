---
title: Ažuriranje DNS zapisa radi održavanja web-mjesta kod trenutnog davatelja usluge hostiranja
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665752"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Ažuriranje DNS zapisa radi održavanja web-mjesta kod trenutnog davatelja usluge hostiranja

1. U centru za administratore sustava Microsoft **Setup**365  >  [otvorite](https://portal.office.com/adminportal/home#/Domains) stranicu Postava domene, a zatim na popisu domena odaberite domenu koju koristite za svoje web-mjesto.

2. Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:

  - Za **unos DNS vrste:** **A (Adresa)**

  - Za **naziv glavnog računala ili pseudonim**upišite sljedeće:**@**

  - Za **IP adresu**upišite statičku IP adresu web-lokacije na kojoj se trenutno hostira (na primjer, 172.16.140.1).

    To mora biti *statička* IP adresa za web-mjesto, a ne *dinamička* IP adresa. Provjerite s web-lokacijom na kojoj se nalazi vaše web-mjesto da biste bili sigurni da možete dobiti statičku IP adresu za javno web-mjesto.

3. Odaberite **Spremi**.

Osim toga, možete stvoriti CNAME zapis da biste korisnicima pomogli pronaći vaše web-mjesto.
  
1. Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:

  - Za **DNS tip** ulaziti: **CNAME (Pseudonim)**

  - Za **naziv glavnog računala ili pseudonim**upišite sljedeće: **www**

  - Za **adrese upućuje na adresu**upišite potpuno kvalificirani naziv domene (FQDN) za web-mjesto (na primjer, contoso.com).

2. Odaberite **Spremi**.
