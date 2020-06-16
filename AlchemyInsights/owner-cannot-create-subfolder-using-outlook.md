---
title: Vlasnik ne može stvoriti podmapu pomoću programa Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748791"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="c8e8c-102">Vlasnik ne može stvoriti podmapu pomoću programa Outlook</span><span class="sxs-lookup"><span data-stu-id="c8e8c-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="c8e8c-103">**Postoji problem s vlasnicima javnih mapa koji stvaraju podmape pomoću programa Outlook. Problem će uskoro biti riješen.**</span><span class="sxs-lookup"><span data-stu-id="c8e8c-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="c8e8c-104">U međuvremenu, koristite jedan od sljedećih zaobilaznih rješenja:</span><span class="sxs-lookup"><span data-stu-id="c8e8c-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="c8e8c-105">Stvaranje podmape pomoću programa Outlook za MAC jer problem utječe samo na Prozore programa Outlook za stolna računala (sve verzije)</span><span class="sxs-lookup"><span data-stu-id="c8e8c-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="c8e8c-106">Imati admin stvoriti podmapu pomoću EXO Shell ili EAC</span><span class="sxs-lookup"><span data-stu-id="c8e8c-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="c8e8c-107">Chanel PropustPublicFolderMailbox/ DjelotvoranPublicFolderMailbox na korisnik to ostali poštanski sandučić nego Izdovoljiti se Poštanski sandučić za savijač uzrokujući ispostavljati</span><span class="sxs-lookup"><span data-stu-id="c8e8c-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="c8e8c-108">*Zalazak- Poštanski sandučić Korisnik1 PropustPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="c8e8c-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="c8e8c-109">Pričekajte sat vremena, ponovno pokrenite outlook klijent</span><span class="sxs-lookup"><span data-stu-id="c8e8c-109">Wait for an hour, restart outlook client</span></span>