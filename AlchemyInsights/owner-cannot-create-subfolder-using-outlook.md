---
title: Vlasnik ne može stvoriti pod-mapu pomoću Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063116"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Vlasnik ne može stvoriti pod-mapu pomoću Outlook

**U tijeku je problem s vlasnicima javnih mapa koji stvaraju podmape pomoću Outlook. Problem će uskoro biti riješen.**

U međuvremenu koristite jedno od sljedećih zaobilaznih rješenja:

1. Pomoću Outlook za MAC stvorite podmapu jer problem utječe samo na Outlook za stolna računala (sve verzije)
2. Stvaranje podmape administratora pomoću ljuske EXO ili EAC
3. Promjena poštanskog sandučića DefaultPublicFolderMailbox/EffectivePublicFolderMailbox na korisniku u drugi poštanski sandučić osim poštanskog sandučića sadržaja za mapu koja uzrokuje problem  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Pričekajte sat vremena, ponovno pokrenite klijent programa Outlook