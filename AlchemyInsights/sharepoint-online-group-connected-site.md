---
title: Dodavanje grupe na SharePoint web-mjesto
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
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770343"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="1d8a1-102">Problemi prilikom stvaranja grupnog povezanog web-mjesta u sustavu SharePoint</span><span class="sxs-lookup"><span data-stu-id="1d8a1-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="1d8a1-103">Neki uobičajeni problemi naišli su pri stvaranju ili ponovnom stvaranju grupe povezanog web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="1d8a1-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="1d8a1-104">Ako ste izbrisali grupu i njegovo povezano web-mjesto i želite stvoriti drugo web-mjesto s istim URL-om, morat ćete trajno ukloniti prethodno web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="1d8a1-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="1d8a1-105">Preuzmite " [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) "</span><span class="sxs-lookup"><span data-stu-id="1d8a1-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="1d8a1-106">Dodatne informacije o tome kako početi s PowerShell potražite u nastavku [programa SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="1d8a1-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="1d8a1-107">Uklonite web-mjesto iz izbrisanih web-mjesta pomoću cmdleta [Ukloni-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1d8a1-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="1d8a1-108">PowerShell je potrebno trajno izbrisati grupe web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="1d8a1-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="1d8a1-109">Ako stvarate grupnu povezanu stranicu i primite upozorenje: **druga grupa s istim pseudonimom već postoji**, provjerite postojeće grupe iz [Office 365 iz centra za administraciju](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="1d8a1-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="1d8a1-110">Da biste riješili problem, izbrišite postojeću grupu ako više nije potrebna ili stvorite web-mjesto s dodijeljenim drugim pseudonimom.</span><span class="sxs-lookup"><span data-stu-id="1d8a1-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="1d8a1-111">Postoje različiti načini stvaranja i korištenja modernih grupa u sustavu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1d8a1-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="1d8a1-112">Postojeća web-mjesta možete povezati s Officeovom 365 grupom.</span><span class="sxs-lookup"><span data-stu-id="1d8a1-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="1d8a1-113">Dodatne informacije potražite [u okviru Povezivanje grupe sustava Office 365 pomoću korisničkog sučelja sustava SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="1d8a1-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="1d8a1-114">Za stvaranje povezanog web-mjesta sustava Office 365, morat ćete stvoriti [timsko web-mjesto](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="1d8a1-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
