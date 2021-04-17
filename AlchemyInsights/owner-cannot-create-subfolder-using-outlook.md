---
title: Vlasnik ne može stvoriti pod-mapu pomoću programa Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836127"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Vlasnik ne može stvoriti pod-mapu pomoću programa Outlook

**U tijeku je problem s vlasnicima javnih mapa koji stvaraju podmape pomoću programa Outlook. Problem će uskoro biti riješen.**

U međuvremenu koristite jedno od sljedećih zaobilaznih rješenja:

1. Stvaranje podmape pomoću programa Outlook za MAC jer problem utječe samo na Outlook za stolna računala (sve verzije)
2. Stvaranje podmape administratora pomoću ljuske EXO ili EAC
3. Promjena poštanskog sandučića DefaultPublicFolderMailbox/EffectivePublicFolderMailbox na korisniku u drugi poštanski sandučić osim poštanskog sandučića sadržaja za mapu koja uzrokuje problem  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Pričekajte sat vremena, ponovno pokrenite klijent programa Outlook