---
title: Pogreška slanja e-pošte blokiran SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30761625"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Pogreška slanja e-pošte: klijent domaćin blokirane pomoću Spamhaus

IP adresu slanja poruke je na popisu blok vlasništvu [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Za blokira Spamhaus razlozi ugrožena račune ugrožena strojeva zajedničko korištenje javne IP adresa i pravila davatelj internetskih usluga (ISP). Mogući popravke su:
  
- Blokirani ulaznih poruka za Office 365 gdje kontrolu izvorni poslužitelj e-pošte, morate odrediti uzrok i uklonite bloka s Spamhaus web-mjesta.
    
- Blokirani ulaznih poruka za Office 365 gdje IP adresu izvora pripada nekom drugom, vlasnik adresa mora ukloniti bloka s Spamhaus web-mjesta. Ako je IP adresa na na pravila blok popisa (PBL), vlasnik možete dodijeliti različite statička IP adresa ili uklanjanje adresu u PBL.
    
- Za blokirane izlaznog poruke iz domenu Office 365, možete primati ovu pogrešku ako poruke usmjeravaju kroz 3 servis proizvođača. Alat za pronalaženje WHOIS možete koristiti za pronalaženje blokirani vlasnik IP adresu.
    

