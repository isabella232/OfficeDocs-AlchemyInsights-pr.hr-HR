---
title: Ograničavanje pristupa u sustavu SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692757"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="b4d03-102">Ograničavanje pristupa u sustavu SharePoint ili OneDrive</span><span class="sxs-lookup"><span data-stu-id="b4d03-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="b4d03-103">Postoji mnogo načina za ograničavanje pristupa servisima sharepoint online/onedrive.</span><span class="sxs-lookup"><span data-stu-id="b4d03-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="b4d03-104">Ove različite metode ograničavanja pristupa navedene su u nastavku.</span><span class="sxs-lookup"><span data-stu-id="b4d03-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="b4d03-105">**Ograničenje dozvole**</span><span class="sxs-lookup"><span data-stu-id="b4d03-105">**Permission Restriction**</span></span>

<span data-ttu-id="b4d03-106">U sustavima SharePoint Online i OneDrive za tvrtke ograničavamo pristup stavkama kao što su web-mjesta, datoteke i mape samo tako što omogućujemo pristup onim grupama/pojedincima koji bi trebali imati pristup.</span><span class="sxs-lookup"><span data-stu-id="b4d03-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="b4d03-107">Prilagodba dozvola za SharePoint popis ili biblioteku</span><span class="sxs-lookup"><span data-stu-id="b4d03-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="b4d03-108">Prilagodba dozvola za web-mjesto sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="b4d03-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="b4d03-109">Promjena dozvola u podmapi</span><span class="sxs-lookup"><span data-stu-id="b4d03-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="b4d03-110">Upravljanje pristupom s neupravljanih uređaja</span><span class="sxs-lookup"><span data-stu-id="b4d03-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="b4d03-111">Kao sharepoint ili globalni administrator možete blokirati ili ograničiti pristup sadržaju sustava SharePoint i OneDrive s neupravljanih uređaja (oni koji se ne pridružuju ili su u skladu s njima u programu Intune).</span><span class="sxs-lookup"><span data-stu-id="b4d03-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="b4d03-112">**Ograničenje mrežnog mjesta**</span><span class="sxs-lookup"><span data-stu-id="b4d03-112">**Network Location Restriction**</span></span>

<span data-ttu-id="b4d03-113">Kao IT administrator možete kontrolirati pristup resursima sustava SharePoint i OneDrive na temelju definiranih mrežnih mjesta koja su vam pouzdana.</span><span class="sxs-lookup"><span data-stu-id="b4d03-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="b4d03-114">To je poznato i kao pravila temeljena na lokaciji.</span><span class="sxs-lookup"><span data-stu-id="b4d03-114">This is also known as location-based policy.</span></span> <span data-ttu-id="b4d03-115">Dodatne informacije potražite u članku [Upravljanje pristupom podacima sustava SharePoint Online i podacima servisa OneDrive na temelju mrežnog mjesta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="b4d03-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="b4d03-116">**Ograničenje zaključavanja web-mjesta**</span><span class="sxs-lookup"><span data-stu-id="b4d03-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="b4d03-117">U sustavu SharePoint Online možete zaključati zbirku web-mjesta, tako da nitko nema pristup.</span><span class="sxs-lookup"><span data-stu-id="b4d03-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="b4d03-118">To je postavljeno putem komponente PowerShell i [ljuske za upravljanje sustavom SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću svojstva [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="b4d03-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="b4d03-119">**Ograničavanje korisnika u stvaranju web-mjesta ili podmjesta**</span><span class="sxs-lookup"><span data-stu-id="b4d03-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="b4d03-120">Kao administrator sustava SharePoint ili globalni administrator možete dopustiti korisnicima stvaranje i administriranje vlastitih web-mjesta sustava SharePoint, određivanje vrsta web-mjesta koja mogu stvoriti i određivanje mjesta web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="b4d03-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="b4d03-121">Dodatne informacije potražite u članku [Upravljanje stvaranjem web-mjesta u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="b4d03-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

