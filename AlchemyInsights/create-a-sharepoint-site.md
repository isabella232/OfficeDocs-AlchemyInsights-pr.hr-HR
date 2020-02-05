---
title: Stvaranje SharePoint web-mjesta
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770847"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="1755d-102">Stvaranje SharePoint web-mjesta</span><span class="sxs-lookup"><span data-stu-id="1755d-102">Create a SharePoint site</span></span>

<span data-ttu-id="1755d-103">Stvaranje web-mjesta iz [aktivnih web-mjesta](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) ili upravljanje njima u centru za administraciju sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1755d-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="1755d-104">Dodatne informacije potražite [u okviru Upravljanje web-lokacijama u novom centru za administraciju sustava SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="1755d-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="1755d-105">Savjeti:</span><span class="sxs-lookup"><span data-stu-id="1755d-105">Tips:</span></span>

- <span data-ttu-id="1755d-106">Ne **možete** stvoriti web-mjesto s istim URL-om postojećeg web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="1755d-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="1755d-107">Ako ste izbrisali web-mjesto i želite ponovno koristiti URL, moguće je da izbrisana stranica još uvijek postoji pod [izbrisanim web-mjestima](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="1755d-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="1755d-108">Web-mjesto će se morati trajno izbrisati da biste ponovno koristili URL.</span><span class="sxs-lookup"><span data-stu-id="1755d-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="1755d-109">Da biste u potpunosti uklonili web-mjesto s PowerShell, Pogledajte primjer " [Ukloni SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) " cmdlet.</span><span class="sxs-lookup"><span data-stu-id="1755d-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="1755d-110">Neki korisnici možda neće moći stvoriti web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="1755d-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="1755d-111">[Pogledajte upravljanje stvaranjem web-mjesta u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="1755d-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="1755d-112">Moguće je da se stranica pojavi zaglavljeno u **stvaranju** duže od očekivanog.</span><span class="sxs-lookup"><span data-stu-id="1755d-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="1755d-113">Ako je prošlo više od 24 sata od kada ste prvi put vidjeli ovaj problem, molimo prijavite ulaznicu za podršku.</span><span class="sxs-lookup"><span data-stu-id="1755d-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="1755d-114">U mnogim slučajevima već radimo na rješenju.</span><span class="sxs-lookup"><span data-stu-id="1755d-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="1755d-115">Molim vas, dajte nam najmanje 24 sata da dovršimo rješenje.</span><span class="sxs-lookup"><span data-stu-id="1755d-115">Please give us at least 24 hours to complete a solution.</span></span>
