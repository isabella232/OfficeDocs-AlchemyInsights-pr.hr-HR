---
title: Povezivanjem SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508415"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="b9e87-102">Povezivanjem SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="b9e87-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="b9e87-103">Ako SharePoint Designer se pojavili problemi veze na SharePoint web-mjesta, pokušajte sljedeća rješenja uobičajenih.</span><span class="sxs-lookup"><span data-stu-id="b9e87-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="b9e87-104">Korak 1: Provjerite je li SharePoint Designer 2013 ažurira s [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [kolovoz 2, 2016 ažuriranje SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="b9e87-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="b9e87-105">Korak 2: Poništite lokalne predmemorije datoteke:</span><span class="sxs-lookup"><span data-stu-id="b9e87-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="b9e87-106">Zatvorite SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="b9e87-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="b9e87-107">Uklanjanje svih datoteka pronađenih u svakoj od sljedećih mapa na lokalnom računalu.</span><span class="sxs-lookup"><span data-stu-id="b9e87-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="b9e87-108">Extensions\Cache %APPDATA%\Microsoft\Web poslužitelj</span><span class="sxs-lookup"><span data-stu-id="b9e87-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="b9e87-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="b9e87-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="b9e87-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="b9e87-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="b9e87-111">Otvorite SharePoint 2013 dizajner i unesite račun da biste vidjeli ako radi.</span><span class="sxs-lookup"><span data-stu-id="b9e87-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="b9e87-112">Korak 3: [Omogući provjeru autentičnosti Moderna 2013 Office na Windows uređajima](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="b9e87-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="b9e87-113">Korak 4: Administratori morat ćete **Dopustiti prilagođene skripte** u postavkama SharePoint administraciju Center dopustiti povezivanje SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="b9e87-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="b9e87-114">Pogledajte [Dopusti ili spriječiti prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) dodatne informacije.</span><span class="sxs-lookup"><span data-stu-id="b9e87-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


