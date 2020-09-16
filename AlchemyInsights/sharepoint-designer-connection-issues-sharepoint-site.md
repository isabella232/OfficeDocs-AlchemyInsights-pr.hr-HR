---
title: Problemi s povezivanjem programa SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727163"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="516be-102">Problemi s povezivanjem programa SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="516be-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="516be-103">Ako SharePoint Designer doživljava probleme s vezom na web-mjesta sustava SharePoint, isprobajte sljedeća najčešća rješenja.</span><span class="sxs-lookup"><span data-stu-id="516be-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="516be-104">Prvi korak: Provjerite je li SharePoint Designer 2013 ažuriran uz [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [kolovoz 2, 2016 Update za SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="516be-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="516be-105">Drugi korak: brisanje lokalnih datoteka predmemorije:</span><span class="sxs-lookup"><span data-stu-id="516be-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="516be-106">Zatvori SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="516be-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="516be-107">Na lokalnom računalu uklonite sve datoteke koje se nalaze u svakoj od sljedećih mapa.</span><span class="sxs-lookup"><span data-stu-id="516be-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="516be-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="516be-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="516be-109">%APPDATA%\Microsoft\SharePoint Designer\proxymontalicache</span><span class="sxs-lookup"><span data-stu-id="516be-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="516be-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="516be-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="516be-111">Otvorite SharePoint Designer 2013 i ponovno unesite račun da biste vidjeli funkcionira li.</span><span class="sxs-lookup"><span data-stu-id="516be-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="516be-112">Treći korak: [Omogućivanje moderne provjere autentičnosti za Office 2013 na uređajima sa sustavom Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="516be-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="516be-113">Četvrti korak: Administratori će morati **dopustiti prilagođenu skriptu** u postavkama centra za administratore sustava SharePoint da bi se omogućila veza programa SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="516be-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="516be-114">Dodatne informacije potražite u članku [Omogućivanje i onemogućivanje prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="516be-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


