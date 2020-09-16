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
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="b2bc9-102">Vlasnik ne može stvoriti podmapu pomoću programa Outlook</span><span class="sxs-lookup"><span data-stu-id="b2bc9-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="b2bc9-103">**U tijeku je problem s vlasnicima javnih mapa koji stvaraju podmape pomoću programa Outlook. Problem će se uskoro popraviti.**</span><span class="sxs-lookup"><span data-stu-id="b2bc9-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="b2bc9-104">U međuvremenu upotrijebite jedno od sljedećih zaobilaznih rješenja:</span><span class="sxs-lookup"><span data-stu-id="b2bc9-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="b2bc9-105">Korištenje programa Outlook za MAC za stvaranje podmape kao problema utječe samo na Outlook za stolna računala u sustavu Windows (sve verzije)</span><span class="sxs-lookup"><span data-stu-id="b2bc9-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="b2bc9-106">Neka administrator stvori podmapu pomoću programa EXO Shell ili EAC</span><span class="sxs-lookup"><span data-stu-id="b2bc9-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="b2bc9-107">Promjena gumba Defaultpublifoldermailbox/Effectivepublifoldermailbox na korisniku s drugim poštanskim sandučićem od poštanskog sandučića sadržaja za mapu koja izaziva problem</span><span class="sxs-lookup"><span data-stu-id="b2bc9-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="b2bc9-108">*Set-Mailbox Korisnik1 Defaultpublifoldermailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="b2bc9-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="b2bc9-109">Pričekajte sat vremena, ponovno pokrenite klijent programa Outlook</span><span class="sxs-lookup"><span data-stu-id="b2bc9-109">Wait for an hour, restart outlook client</span></span>