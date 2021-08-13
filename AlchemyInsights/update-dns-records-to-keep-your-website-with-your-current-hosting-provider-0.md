---
title: Ažuriranje DNS zapisa da biste web-mjesto održavali kod trenutnog davatelja usluge hostiranja
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007674"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Ažuriranje DNS zapisa da biste web-mjesto održavali kod trenutnog davatelja usluge hostiranja

1. Na Centar za administratore okruženja Microsoft 365 odaberite **stranicu Postavljanje** domena, a zatim na popisu domena odaberite  >  [](https://admin.microsoft.com/Adminportal#/Domains) domenu koju koristite za web-mjesto.

2. Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:

  - Za **unos vrste DNS:A** **(Adresa)**

  - U **naziv glavnog računala ili Pseudonim** upišite sljedeće: **@**

  - Za **IP adresu** upišite statičnu IP adresu za web-mjesto na kojem se trenutno hostira (npr. 172.16.140.1).

    To mora biti  *statična*  IP adresa za web-mjesto, a ne  *dinamička*  IP adresa. Provjerite s web-mjestom na kojem se hostira vaše web-mjesto da biste bili sigurni da možete dobiti statičnu IP adresu za javno web-mjesto.

3. Odaberite **Spremi**.

Osim toga, možete stvoriti CNAME zapis da biste korisnicima pomogli pronaći vaše web-mjesto.
  
1. Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:

  - Za **vrstu DNS-a** unesite: **CNAME (pseudonim)**

  - Za **naziv glavnog računala ili Pseudonim** upišite sljedeće: **www**

  - U **okvir Upućuje na adresu** upišite potpuno kvalificirani naziv domene (FQDN) za web-mjesto (npr. contoso.com).

2. Odaberite **Spremi**.
