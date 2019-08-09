---
title: Stvaranje SharePoint web-mjesta
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ad1a77b69d2d453dbd3daa304759238b329f96ba
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269908"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="3b2c6-102">Stvaranje SharePoint web-mjesta</span><span class="sxs-lookup"><span data-stu-id="3b2c6-102">Create a SharePoint site</span></span>

<span data-ttu-id="3b2c6-103">Možete vidjeti sljedeće informacije o stvaranja web-mjesta SharePoint:</span><span class="sxs-lookup"><span data-stu-id="3b2c6-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="3b2c6-104">[Upravljanje web-mjestima u novi centar admin SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Saznajte više o mogućnosti stvaranja web-mjesta, uključujući kako stvoriti Klasična web-mjesta ili web-mjesto za timove koji ne uključuje grupe Office 365.</span><span class="sxs-lookup"><span data-stu-id="3b2c6-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="3b2c6-105">[Stvori web-mjesto tima u SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Saznajte kako stvoriti web-mjesto tima.</span><span class="sxs-lookup"><span data-stu-id="3b2c6-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="3b2c6-106">[Stvaranje web-mjesta komunikacije u SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Saznajte kako stvoriti komunikacijski web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="3b2c6-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="3b2c6-107">[Upravljanje web-mjestima u novi centar admin SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Saznajte kako stvoriti Klasična web-mjesta ili web-mjesto tima koji ne uključuje grupe Office 365.</span><span class="sxs-lookup"><span data-stu-id="3b2c6-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Savjeti]
> - <span data-ttu-id="3b2c6-109">Nije moguće stvoriti web-mjesto s istim URL postojećeg web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="3b2c6-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="3b2c6-110">Ako brišu web-mjesta i želimo da ponovno koristite URL, moguće je izbrisano web-mjesto još uvijek postoji pod **Izbrisano web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="3b2c6-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="3b2c6-111">Upravljanje izbrisati web-mjesta pogledajte [Brisanje web-mjesta](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="3b2c6-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="3b2c6-112">Da biste potpuno uklonili web-mjesto Powershell pogledajte primjer cmdlet [Ukloni SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="3b2c6-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="3b2c6-113">Neki korisnici možda neće moći stvoriti web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="3b2c6-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="3b2c6-114">Pogledajte [Stvaranje web-mjesta upravljanje u SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="3b2c6-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="3b2c6-115">Moguće je web-mjesto se pojavljuje stuck na **Stvaranje** dulje od očekivanog.</span><span class="sxs-lookup"><span data-stu-id="3b2c6-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="3b2c6-116">Ako više od 24 sata prošlo Budući vidjeli taj problem, prijaviti ulaznica za podršku.</span><span class="sxs-lookup"><span data-stu-id="3b2c6-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="3b2c6-117">U mnogim slučajevima smo već radite rješenje.</span><span class="sxs-lookup"><span data-stu-id="3b2c6-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="3b2c6-118">Molimo pošaljite nam najmanje 24 sata dovršiti rješenje.</span><span class="sxs-lookup"><span data-stu-id="3b2c6-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="3b2c6-119">Ako trebate stvoriti nova web-mjesta tima koji ne uključuje Office 365 grupi</span><span class="sxs-lookup"><span data-stu-id="3b2c6-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


