---
title: Ograničiti pristup u SharePoint ili OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735135"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="69384-102">Ograničiti pristup u SharePoint ili OneDrive</span><span class="sxs-lookup"><span data-stu-id="69384-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="69384-103">Postoji mnogo načina ograničiti pristup Internetu OneDrive SharePoint services.</span><span class="sxs-lookup"><span data-stu-id="69384-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="69384-104">Ove različite metode ograničenje pristupa istaknuti su ispod.</span><span class="sxs-lookup"><span data-stu-id="69384-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="69384-105">Ograničenje dozvola</span><span class="sxs-lookup"><span data-stu-id="69384-105">Permission Restriction</span></span>

<span data-ttu-id="69384-106">U SharePoint Online i OneDrive za poslovne, možemo ograničiti pristup stavki kao što su web-mjesta, datoteke i mape samo Davanjem pristup tim grupama/pojedinaca koji treba imati pristup.</span><span class="sxs-lookup"><span data-stu-id="69384-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

[<span data-ttu-id="69384-107">Prilagodba dozvola za SharePoint popis ili biblioteku</span><span class="sxs-lookup"><span data-stu-id="69384-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[<span data-ttu-id="69384-108">Prilagodba dozvola SharePoint web-mjesta</span><span class="sxs-lookup"><span data-stu-id="69384-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[<span data-ttu-id="69384-109">Promijenite dozvole na podmapi</span><span class="sxs-lookup"><span data-stu-id="69384-109">Change the permissions on a subfolder</span></span>](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[<span data-ttu-id="69384-110">Kontrolu pristupa iz neupravljanog uređaja</span><span class="sxs-lookup"><span data-stu-id="69384-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="69384-111">Kao SharePoint ili globalni administrator sistema Office 365, možete blokirati ili ograničiti pristup SharePoint i OneDrive sadržaja iz neupravljanog uređaja (one ne hibridno AD spojena ili sa standardom u Intune).</span><span class="sxs-lookup"><span data-stu-id="69384-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="69384-112">Mrežni mjesto ograničenja</span><span class="sxs-lookup"><span data-stu-id="69384-112">Network Location Restriction</span></span>

<span data-ttu-id="69384-113">Kao IT administrator, možete kontrolirati pristup resursima sustava SharePoint i OneDrive na temelju definiranih mrežnim mjestima kojima vjerujete.</span><span class="sxs-lookup"><span data-stu-id="69384-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="69384-114">To je poznato kao mjesto temelji pravila.</span><span class="sxs-lookup"><span data-stu-id="69384-114">This is also known as location-based policy.</span></span> <span data-ttu-id="69384-115">Za dodatne informacije pogledajte [pristup kontrolu SharePoint Online i OneDrive podatke na temelju mrežnog mjesta](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="69384-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="69384-116">Ograničenje zaključavanja web-mjesta</span><span class="sxs-lookup"><span data-stu-id="69384-116">Site Lock Restriction</span></span> 

<span data-ttu-id="69384-117">Unutar SharePoint Online imaju mogućnost za zaključavanje zbirke web-mjesta tako da nitko ima pristup.</span><span class="sxs-lookup"><span data-stu-id="69384-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="69384-118">Postavljena je putem PowerShell i [Online ljuske za upravljanje SharePoint](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću svojstva - stanje zaključanosti [Skup SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="69384-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="69384-119">Ograničenje korisnika u stvaranju web-mjesta ili podmjesta</span><span class="sxs-lookup"><span data-stu-id="69384-119">Restrict users from creating sites or subsites</span></span>

<span data-ttu-id="69384-120">Kao administraciju SharePoint ili globalni administrator sistema Office 365, možete dopustiti korisnicima stvaranje i administrirati vlastite SharePoint web-mjesta, odredite Kakvu vrstu web-mjesta mogu stvoriti, i navedite mjesto web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="69384-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="69384-121">Za dodatne informacije pogledajte [Upravljanje stvaranja web-mjesta u SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="69384-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span></span>

