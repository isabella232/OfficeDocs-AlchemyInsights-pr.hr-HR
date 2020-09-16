---
title: Vlasnik ne može stvoriti podmapu pomoću programa Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665710"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Vlasnik ne može stvoriti podmapu pomoću programa Outlook

**U tijeku je problem s vlasnicima javnih mapa koji stvaraju podmape pomoću programa Outlook. Problem će se uskoro popraviti.**

U međuvremenu upotrijebite jedno od sljedećih zaobilaznih rješenja:

1. Korištenje programa Outlook za MAC za stvaranje podmape kao problema utječe samo na Outlook za stolna računala u sustavu Windows (sve verzije)
2. Neka administrator stvori podmapu pomoću programa EXO Shell ili EAC
3. Promjena gumba Defaultpublifoldermailbox/Effectivepublifoldermailbox na korisniku s drugim poštanskim sandučićem od poštanskog sandučića sadržaja za mapu koja izaziva problem  
    - *Set-Mailbox Korisnik1 Defaultpublifoldermailbox PubMBX3*
4. Pričekajte sat vremena, ponovno pokrenite klijent programa Outlook