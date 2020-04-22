---
title: Ograničavanje pristupa u sustavu SharePoint ili OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715876"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="376c7-102">Ograničavanje pristupa u sustavu SharePoint ili OneDrive</span><span class="sxs-lookup"><span data-stu-id="376c7-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="376c7-103">U sustavima SharePoint i OneDrive ograničavate pristup stavkama kao što su datoteke, mape i popisi dodjelom pristupa samo grupama ili pojedincima kojima želite pristupiti.</span><span class="sxs-lookup"><span data-stu-id="376c7-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="376c7-104">Prema zadanim postavkama dozvole u sustavu SharePoint nasljeđuju se od višeg položaja u hijerarhiji.</span><span class="sxs-lookup"><span data-stu-id="376c7-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="376c7-105">Dakle, datoteka nasljeđuje dozvole iz mape, koja nasljeđuje dozvole iz biblioteke, koja nasljeđuje svoje dozvole od web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="376c7-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="376c7-106">Možete dijeliti na višoj razini (primjerice dijeljenjem cijelog web-mjesta), a zatim prekinuti nasljeđivanje ako ne želite dijeliti sve stavke na web-mjestu.</span><span class="sxs-lookup"><span data-stu-id="376c7-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="376c7-107">Međutim, to ne preporučujemo jer održavanje dozvola čini složenijim i zbunjujućijima u budućnosti.</span><span class="sxs-lookup"><span data-stu-id="376c7-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="376c7-108">Evo što možete učiniti umjesto toga:</span><span class="sxs-lookup"><span data-stu-id="376c7-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="376c7-109">Ako, na primjer, želite zajednički koristiti sav sadržaj mape osim jedne datoteke u njoj, premjestite je na novo mjesto koje nije dijeljeno.</span><span class="sxs-lookup"><span data-stu-id="376c7-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="376c7-110">Ako u mapi imate dvije podmape i želite zajednički koristiti jednu podmapu s grupama A i B i dopustiti samo grupni pristup drugoj podmapi, podijelite nadređenu mapu s grupom A i dodajte grupu B u prvu podmapu.</span><span class="sxs-lookup"><span data-stu-id="376c7-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="376c7-111">Prekid zajedničkog korištenja datoteke ili mape</span><span class="sxs-lookup"><span data-stu-id="376c7-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

