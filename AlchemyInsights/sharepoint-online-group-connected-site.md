---
title: Dodavanje grupe na web-mjesto sustava SharePoint
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
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771191"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="320af-102">Problemi prilikom stvaranja grupnog povezanog web-mjesta u sustavu SharePoint</span><span class="sxs-lookup"><span data-stu-id="320af-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="320af-103">Neki se Česti problemi susreću prilikom stvaranja ili ponovnog stvaranja grupnog povezanog web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="320af-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="320af-104">Ako ste izbrisali grupu i njegovo povezano web-mjesto i želite stvoriti drugo web-mjesto s istim URL-om, morat ćete trajno ukloniti prethodno web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="320af-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="320af-105">Preuzimanje [ljuske za upravljanje SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) -om</span><span class="sxs-lookup"><span data-stu-id="320af-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="320af-106">Dodatne informacije o pokretanju pomoću komponente PowerShell potražite u članku [početak rada s ljuskom za upravljanje sustavom SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="320af-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="320af-107">Uklonite web-mjesto s izbrisanih web-mjesta pomoću cmdleta [Remove-Spodeletedweb](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="320af-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="320af-108">PowerShell je dužan trajno izbrisati grupna web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="320af-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="320af-109">Ako stvarate grupno povezano web-mjesto i primate upozorenje: **druga grupa s istim pseudonimom već postoji**, provjerite postojeće grupe iz centra za [administratore sustava Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="320af-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="320af-110">Da biste riješili problem, izbrišite postojeću grupu ako više nije potrebna ili stvorite web-mjesto s dodijeljenim drugim pseudonimom.</span><span class="sxs-lookup"><span data-stu-id="320af-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="320af-111">Postoje razni načini stvaranja i korištenja suvremenih grupa u sustavu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="320af-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="320af-112">Možete povezati postojeća web-mjesta s grupom Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="320af-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="320af-113">Dodatne informacije potražite u članku [Povezivanje grupe Microsoft 365 pomoću korisničkog sučelja sustava SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="320af-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="320af-114">Da biste stvorili web-mjesto povezanih s grupom Microsoft 365, morat ćete stvoriti [timsko web-mjesto](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="320af-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
