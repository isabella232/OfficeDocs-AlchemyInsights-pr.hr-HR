---
title: Ograničavanje pristupa u sustavu SharePoint ili na servisu OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720674"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="afba6-102">Ograničavanje pristupa u sustavu SharePoint ili na servisu OneDrive</span><span class="sxs-lookup"><span data-stu-id="afba6-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="afba6-103">U sustavu SharePoint i na servisu OneDrive ograničite pristup stavkama kao što su datoteke, mape i popisi tako da pristupate samo grupama ili pojedincima kojima želite pristupiti.</span><span class="sxs-lookup"><span data-stu-id="afba6-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="afba6-104">Dozvole u sustavu SharePoint po zadanom se nasljeđuju od viših prema gore u hijerarhiji.</span><span class="sxs-lookup"><span data-stu-id="afba6-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="afba6-105">Tako da datoteka nasljeđuje dozvole iz mape, koja nasljeđuje dozvole iz biblioteke, koja nasljeđuje dozvole od web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="afba6-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="afba6-106">Možete zajednički koristiti na višoj razini (kao što je zajedničko korištenje cijelog web-mjesta), a zatim prekinuti nasljeđivanje ako ne želite zajednički koristiti sve stavke na web-mjestu.</span><span class="sxs-lookup"><span data-stu-id="afba6-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="afba6-107">No to ne preporučujemo jer čini održavanje dozvola složenijim i dvosmislenim u budućnosti.</span><span class="sxs-lookup"><span data-stu-id="afba6-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="afba6-108">Evo što možete učiniti:</span><span class="sxs-lookup"><span data-stu-id="afba6-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="afba6-109">Ako, primjerice, želite zajednički koristiti sve sadržaje mape osim jedne datoteke u njoj, premjestite je na novo mjesto koje se ne zajednički koristi.</span><span class="sxs-lookup"><span data-stu-id="afba6-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="afba6-110">Ako u mapi imate dvije podmape, a želite zajednički koristiti jednu podmapu s grupama A i B te dopustiti samo grupu pristupa drugoj podmapi, zajednički koristite nadređenu mapu s grupom a i dodajte grupu B u prvu podmapu.</span><span class="sxs-lookup"><span data-stu-id="afba6-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="afba6-111">Prestanak zajedničkog korištenja datoteke ili mape </span><span class="sxs-lookup"><span data-stu-id="afba6-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

