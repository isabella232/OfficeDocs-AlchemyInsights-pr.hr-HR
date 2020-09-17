---
title: Stvaranje web-mjesta sustava SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806931"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="d1d89-102">Stvaranje web-mjesta sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="d1d89-102">Create a SharePoint site</span></span>

<span data-ttu-id="d1d89-103">Stvaranje web-mjesta i upravljanje njima s [aktivnih web-mjesta](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) u centru za administratore sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="d1d89-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="d1d89-104">Dodatne informacije potražite u članku [Upravljanje web-mjestima u novom centru za administratore sustava SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="d1d89-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="d1d89-105">Savjeti</span><span class="sxs-lookup"><span data-stu-id="d1d89-105">Tips:</span></span>

- <span data-ttu-id="d1d89-106">Ne **možete** stvoriti web-mjesto s istim URL-om postojećeg web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="d1d89-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="d1d89-107">Ako ste izbrisali web-mjesto i želite ponovno koristiti URL, moguće je da izbrisane web-mjesto i dalje postoji u odjeljku [Izbrisane web-mjesta](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="d1d89-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="d1d89-108">Web-mjesto će se morati trajno izbrisati da bi se ponovno koristila URL.</span><span class="sxs-lookup"><span data-stu-id="d1d89-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="d1d89-109">Da biste u potpunosti uklonili web-mjesto pomoću komponente PowerShell, pročitajte primjer sustava cmdlet [Remove-SPWeb](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="d1d89-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="d1d89-110">Neki korisnici možda neće moći stvoriti web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="d1d89-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="d1d89-111">[Pročitajte članak upravljanje stvaranjem web-mjesta u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="d1d89-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="d1d89-112">Moguće je da se web-mjesto zapelo pri **stvaranju** više od očekivanog.</span><span class="sxs-lookup"><span data-stu-id="d1d89-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="d1d89-113">Ako je prošlo više od 24 sata otkad ste prvi put vidjeli taj problem, prijavite karticu za podršku.</span><span class="sxs-lookup"><span data-stu-id="d1d89-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="d1d89-114">U mnogim slučajevima već radimo na rješenju.</span><span class="sxs-lookup"><span data-stu-id="d1d89-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="d1d89-115">Dodajte nam najmanje 24 sata da biste dovršili rješenje.</span><span class="sxs-lookup"><span data-stu-id="d1d89-115">Please give us at least 24 hours to complete a solution.</span></span>
