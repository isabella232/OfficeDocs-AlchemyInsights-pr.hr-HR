---
title: Ažuriranje zapisa DNS zadržati svoje web-mjesto s trenutnom pružatelju usluge
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29461768"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Ažuriranje zapisa DNS zadržati svoje web-mjesto s trenutnom pružatelju usluge

1. Na stranici [domena](https://portal.office.com/adminportal/home#/Domains) popisa domena, odaberite domene koristite za vaše web-mjesto, a zatim odaberite **postavke DNS** u okno upravljanje. 
    
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
    

