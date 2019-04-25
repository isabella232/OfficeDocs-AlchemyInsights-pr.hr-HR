---
title: Ograničiti pristup u SharePoint ili OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383863"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="414d9-102">Ograničiti pristup u SharePoint ili OneDrive</span><span class="sxs-lookup"><span data-stu-id="414d9-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="414d9-103">U SharePoint i OneDrive, ograničiti pristup stavki kao što su datoteke, mape i popisa tako da pristup dozvolite samo grupe ili pojedinci želite imati pristup.</span><span class="sxs-lookup"><span data-stu-id="414d9-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="414d9-104">Po zadanom, dozvole u SharePoint nasljeđuju od gore viši u hijerarhiji.</span><span class="sxs-lookup"><span data-stu-id="414d9-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="414d9-105">Stoga datoteku svoje dozvole nasljeđuju od mapa nasljeđuje dozvole iz biblioteke koji svoje dozvole nasljeđuju od web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="414d9-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="414d9-106">Možete zajednički koristiti na višoj razini (kao što su po zajedničko korištenje cijelo web-mjesto) i ukinuti nasljeđivanje ako želite zajednički koristiti stavke na web-mjestu.</span><span class="sxs-lookup"><span data-stu-id="414d9-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="414d9-107">Međutim, ne preporučujemo ovo jer olakšava održavanje dozvola kompleksne i zbunjujuće u budućnosti.</span><span class="sxs-lookup"><span data-stu-id="414d9-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="414d9-108">Evo što nije moguće učiniti umjesto toga:</span><span class="sxs-lookup"><span data-stu-id="414d9-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="414d9-109">Ako, na primjer, želite zajednički koristiti sadržaj mape osim jedne datoteke u njoj, premještanje te datoteke na novo mjesto nije zajednički.</span><span class="sxs-lookup"><span data-stu-id="414d9-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="414d9-110">Ako imate dva podmape u mapi i želite dijeliti jednu podmapu s grupama A i B i dopustiti samo pristup grupi A drugi podmapu, dijeliti nadređene mape s grupom A i dodavanje grupe B prvu podmapu.</span><span class="sxs-lookup"><span data-stu-id="414d9-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="414d9-111">Prekid zajedničkog korištenja datoteke ili mape</span><span class="sxs-lookup"><span data-stu-id="414d9-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

