---
title: Na ovom web-mjestu nije moguće doći do pogreške prilikom pokušaja pristupanja web-mjestu sustava SharePoint iz preglednika ili timova
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 451544fb85522e0eececc9274825805699685ee9
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743439"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a><span data-ttu-id="51bb7-102">Pogreška "nije moguće doći do tog web-mjesta" prilikom pokušaja pristupanja web-mjestu sustava SharePoint iz preglednika ili timova</span><span class="sxs-lookup"><span data-stu-id="51bb7-102">“This site can’t be reached” error when trying to access SharePoint site from browser or Teams</span></span>

<span data-ttu-id="51bb7-103">Prilikom pokušaja pristupanja web-mjestu sustava SharePoint u pregledniku ili timovima, korisnici mogu primiti pogrešku "ovo web-mjesto nije moguće dosegnuti".</span><span class="sxs-lookup"><span data-stu-id="51bb7-103">Users might receive "This site can't be reached" error when trying to access SharePoint site from browser or Teams.</span></span> 

<span data-ttu-id="51bb7-104">Da biste riješili taj problem, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="51bb7-104">To resolve this issue:</span></span> 

1. <span data-ttu-id="51bb7-105">Provjerite je li Početna stranica u smeću koša za smeće ili u košu za smeće druge faze i vratite stranicu.</span><span class="sxs-lookup"><span data-stu-id="51bb7-105">Check if the home page is in Recycle bin or second-stage recycle bin and restore the page.</span></span>

<span data-ttu-id="51bb7-106">**Ogledni Direktni URL za koš za smeće**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="51bb7-106">**Sample direct URL to recycle bin**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>

1. <span data-ttu-id="51bb7-107">Ako se Početna stranica trajno uklanja iz koša za smeće, stvorite novu stranicu web-mjesta iz biblioteke stranica web-mjesta i napravite je kao početnu stranicu.</span><span class="sxs-lookup"><span data-stu-id="51bb7-107">If the home page is permanently removed from the recycle bin, create a new site page from the Site Pages library and make it a homepage.</span></span> 

<span data-ttu-id="51bb7-108">**Ogledni Direktni URL**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="51bb7-108">**Sample direct URL**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>