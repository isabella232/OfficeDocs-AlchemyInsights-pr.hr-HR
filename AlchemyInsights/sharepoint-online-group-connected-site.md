---
title: Dodavanje grupe na Web-mjesto sustava SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44064385"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="0149a-102">Problemi prilikom stvaranja web-mjesta povezanog grupe u sustavu SharePoint</span><span class="sxs-lookup"><span data-stu-id="0149a-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="0149a-103">Neki uobičajeni problemi na koje se susreću prilikom stvaranja ili ponovnog stvaranja povezanog web-mjesta grupe.</span><span class="sxs-lookup"><span data-stu-id="0149a-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="0149a-104">Ako ste izbrisali grupu i povezano web-mjesto i želite stvoriti drugo web-mjesto s istim URL-om, morat ćete trajno ukloniti prethodno web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="0149a-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="0149a-105">Preuzimanje [datoteka SPO Uprava Ljuska](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="0149a-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="0149a-106">Dodatne informacije o početku rada s powershellom potražite u članku [Početak rada s ljuskom za upravljanje sustavom SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="0149a-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="0149a-107">Uklonite web-mjesto s izbrisanih web-mjesta pomoću cmdleta [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell.</span><span class="sxs-lookup"><span data-stu-id="0149a-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="0149a-108">Powershell je potrebno trajno izbrisati grupna web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="0149a-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="0149a-109">Ako stvarate povezano web-mjesto grupe i primate upozorenje: **Još jedna grupa s istim pseudonimom već postoji**, provjerite postojeće grupe iz centra za [administratore sustava Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="0149a-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="0149a-110">Da biste riješili problem, izbrišite postojeću grupu ako više nije potrebna ili stvorite web-mjesto s dodijeljenim drugim pseudonimom.</span><span class="sxs-lookup"><span data-stu-id="0149a-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="0149a-111">Postoje različiti načini stvaranja i korištenja modernih grupa u sustavu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0149a-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="0149a-112">Postojeća web-mjesta možete povezati s grupom microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0149a-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="0149a-113">Dodatne informacije potražite [u odjeljku Povezivanje grupe sustava Microsoft 365 pomoću korisničkog sučelja sustava SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="0149a-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="0149a-114">Da biste stvorili povezano web-mjesto grupe Microsoft 365, morat ćete stvoriti [timsko web-mjesto](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="0149a-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
