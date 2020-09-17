---
title: Ažuriranje DNS zapisa radi zadržavanja web-mjesta s trenutnim davatelja usluga hostiranja
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815777"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Ažuriranje DNS zapisa radi zadržavanja web-mjesta s trenutnim davatelja usluga hostiranja

1. U centru za administratore sustava Microsoft 365 otvorite stranicu **Postavke**  >  [domene](https://admin.microsoft.com/Adminportal#/Domains) , a zatim na popisu domena odaberite domenu koju koristite za web-mjesto.

2. Odaberite **+ novi prilagođeni zapis** pa unesite sljedeće:

  - Za **vrstu DNS** -A unesite: **A (adresa)**

  - Za **naziv glavnog računala ili pseudonim**upišite sljedeće: **@**

  - Za **IP adresu**upišite STATIČNU IP adresu web-mjesta na kojoj je trenutno domaćin (na primjer,: 172.16.140.1).

    Ovo mora biti  *statična*  IP adresa za web-mjesto, a ne  *dinamička*  IP adresa. Provjerite uz web-mjesto na kojem je web-mjesto hostirano da biste mogli nabaviti statičnu IP adresu za javno web-mjesto.

3. Odaberite **Spremi**.

Osim toga, možete stvoriti CNAME zapis koji korisnicima olakšava pronalaženje web-mjesta.
  
1. Odaberite **+ novi prilagođeni zapis** pa unesite sljedeće:

  - Za **vrstu DNS** -a unesite: **CNAME (pseudonim)**

  - Za **naziv glavnog računala ili pseudonim**upišite sljedeće: **www**

  - Da **biste unijeli točku na adresu**, upišite potpuno kvalificirani naziv domene (FQDN) za vaše web-mjesto (primjerice, contoso.com).

2. Odaberite **Spremi**.
