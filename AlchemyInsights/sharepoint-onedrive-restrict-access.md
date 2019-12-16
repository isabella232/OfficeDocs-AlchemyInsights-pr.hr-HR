---
title: Ograničavanje pristupa u sustavu SharePoint ili servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053757"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="439d0-102">Ograničavanje pristupa u sustavu SharePoint ili servisu OneDrive</span><span class="sxs-lookup"><span data-stu-id="439d0-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="439d0-103">Postoji mnogo načina ograničavanja pristupa uslugama SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="439d0-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="439d0-104">Ove različite metode ograničavanja pristupa navedene su u nastavku.</span><span class="sxs-lookup"><span data-stu-id="439d0-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="439d0-105">**Ograničenje dopuštenja**</span><span class="sxs-lookup"><span data-stu-id="439d0-105">**Permission Restriction**</span></span>

<span data-ttu-id="439d0-106">U sustavu SharePoint online i servisu OneDrive za tvrtke ograničavamo pristup stavkama kao što su web-mjesta, datoteke i mape samo dajući pristup tim grupama/pojedincima koji bi trebali imati pristup.</span><span class="sxs-lookup"><span data-stu-id="439d0-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="439d0-107">Prilagodba dozvola za SharePointov popis ili biblioteku</span><span class="sxs-lookup"><span data-stu-id="439d0-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="439d0-108">Prilagodba dozvola web-mjesta sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="439d0-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="439d0-109">Promjena dozvola u podmapi</span><span class="sxs-lookup"><span data-stu-id="439d0-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="439d0-110">Upravljanje pristupom s neupravljanih uređaja</span><span class="sxs-lookup"><span data-stu-id="439d0-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="439d0-111">Kao SharePoint ili Global admin u sustavu Office 365, možete blokirati ili ograničiti pristup sadržaju sustava SharePoint i OneDrive s neupravljanih uređaja (oni koji nisu hibridni AD spojeni ili usklađeni u Intune).</span><span class="sxs-lookup"><span data-stu-id="439d0-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="439d0-112">**Ograničenje mrežnog mjesta**</span><span class="sxs-lookup"><span data-stu-id="439d0-112">**Network Location Restriction**</span></span>

<span data-ttu-id="439d0-113">Kao IT admin možete kontrolirati pristup resursima sustava SharePoint i OneDrive na temelju definiranih mrežnih mjesta kojima vjerujete.</span><span class="sxs-lookup"><span data-stu-id="439d0-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="439d0-114">To se također naziva politikom temeljenom na lokaciji.</span><span class="sxs-lookup"><span data-stu-id="439d0-114">This is also known as location-based policy.</span></span> <span data-ttu-id="439d0-115">Dodatne informacije potražite u [kontroli pristupa podacima sustava SharePoint online i servisu OneDrive na temelju mrežnog mjesta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="439d0-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="439d0-116">**Ograničenje zaključavanja web-mjesta**</span><span class="sxs-lookup"><span data-stu-id="439d0-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="439d0-117">U sustavu SharePoint Online imate mogućnost zaključavanja zbirke web-mjesta, tako da nitko nema pristup.</span><span class="sxs-lookup"><span data-stu-id="439d0-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="439d0-118">To je postavljeno putem PowerShell i [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću [skup-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate svojstvo.</span><span class="sxs-lookup"><span data-stu-id="439d0-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="439d0-119">**Ograničavanje korisnika na stvaranje web-mjesta ili podmjesta**</span><span class="sxs-lookup"><span data-stu-id="439d0-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="439d0-120">Kao administrator sustava SharePoint ili Office 365 Global admin, možete dopustiti korisnicima stvaranje i administriranje vlastitih web-mjesta sustava SharePoint, odrediti koja vrsta web-mjesta mogu stvoriti i odrediti mjesto web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="439d0-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="439d0-121">Dodatne informacije potražite [u okviru Upravljanje stvaranjem web-mjesta u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="439d0-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

