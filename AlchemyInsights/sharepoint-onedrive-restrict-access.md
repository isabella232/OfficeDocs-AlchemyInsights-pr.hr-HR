---
title: Ograničavanje pristupa u sustavu SharePoint ili na servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700447"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="a41c4-102">Ograničavanje pristupa u sustavu SharePoint ili na servisu OneDrive</span><span class="sxs-lookup"><span data-stu-id="a41c4-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="a41c4-103">Postoji mnogo načina ograničavanja pristupa servisima sustava SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a41c4-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="a41c4-104">U nastavku su navedene različite metode ograničavanja pristupa.</span><span class="sxs-lookup"><span data-stu-id="a41c4-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="a41c4-105">**Ograničenje dozvola**</span><span class="sxs-lookup"><span data-stu-id="a41c4-105">**Permission Restriction**</span></span>

<span data-ttu-id="a41c4-106">U sustavima SharePoint online i OneDrive za tvrtke ograničavamo pristup stavkama kao što su web-mjesta, datoteke i mape samo ako dajemo pristup tim grupama/pojedincima koji bi trebali imati pristup.</span><span class="sxs-lookup"><span data-stu-id="a41c4-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="a41c4-107">Prilagodba dozvola za popis ili biblioteku sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="a41c4-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="a41c4-108">Prilagodba dozvola web-mjesta sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="a41c4-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="a41c4-109">Promjena dozvola na podmapi</span><span class="sxs-lookup"><span data-stu-id="a41c4-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="a41c4-110">Upravljanje pristupom iz neupravljanih uređaja</span><span class="sxs-lookup"><span data-stu-id="a41c4-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="a41c4-111">Kao SharePoint ili globalni administrator možete blokirati ili ograničiti pristup sadržaju sustava SharePoint i na servisu OneDrive iz neupravljanih uređaja (one koji nisu hibrid ili kompatibilni u programu Intune).</span><span class="sxs-lookup"><span data-stu-id="a41c4-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="a41c4-112">**Ograničenje mrežnog mjesta**</span><span class="sxs-lookup"><span data-stu-id="a41c4-112">**Network Location Restriction**</span></span>

<span data-ttu-id="a41c4-113">Kao IT administrator možete kontrolirati pristup resursima sustava SharePoint i servisu OneDrive na temelju definiranih mrežnih mjesta kojima vjerujete.</span><span class="sxs-lookup"><span data-stu-id="a41c4-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="a41c4-114">To je poznato i kao pravilo utemeljeno na lokaciji.</span><span class="sxs-lookup"><span data-stu-id="a41c4-114">This is also known as location-based policy.</span></span> <span data-ttu-id="a41c4-115">Dodatne informacije potražite [u članku Upravljanje pristupom na podatke sustava SharePoint online i na servisu OneDrive na temelju mrežnog mjesta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="a41c4-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="a41c4-116">**Ograničenje zaključavanja web-mjesta**</span><span class="sxs-lookup"><span data-stu-id="a41c4-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="a41c4-117">U sustavu SharePoint Online možete zaključati zbirku web-mjesta, pa nitko ne može pristupiti.</span><span class="sxs-lookup"><span data-stu-id="a41c4-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="a41c4-118">Ovo je postavljeno putem komponente PowerShell i [ljuske za upravljanje sustavom SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću svojstva [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="a41c4-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="a41c4-119">**Ograničavanje korisnika na stvaranje web-mjesta ili podmjesta**</span><span class="sxs-lookup"><span data-stu-id="a41c4-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="a41c4-120">Kao administrator sustava SharePoint ili globalni administrator korisnicima možete omogućiti stvaranje i administriranje vlastitih web-mjesta sustava SharePoint, određivanje vrsta web-mjesta koje mogu stvarati i određivanje mjesta web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="a41c4-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="a41c4-121">Dodatne informacije potražite [u članku Upravljanje stvaranjem web-mjesta u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="a41c4-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

