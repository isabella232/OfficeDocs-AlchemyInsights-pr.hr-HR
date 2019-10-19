---
title: Dodavanje grupe na SharePoint web-mjesto
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750512"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="cc50c-102">Problemi pri stvaranju ili grupiranju povezanih web-mjesta u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="cc50c-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="cc50c-103">Došlo je do nekoliko uobičajenih problema pri stvaranju ili ponovnom stvaranju grupe povezanog web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="cc50c-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="cc50c-104">Ako ste izbrisali grupu i njegovo povezano web-mjesto i želite stvoriti drugo web-mjesto s istim URL-om, morat ćete trajno ukloniti prethodno web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="cc50c-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="cc50c-105">Preuzmite " [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) "</span><span class="sxs-lookup"><span data-stu-id="cc50c-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="cc50c-106">Dodatne informacije o početku rada s PowerShell potražite u nastavku [programa SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="cc50c-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="cc50c-107">Uklonite web-mjesto iz izbrisanih web-mjesta pomoću cmdleta [Ukloni-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cc50c-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="cc50c-108">Ako stvarate grupnu povezanu stranicu i primite upozorenje druga grupa s istim pseudonimom već postoji, provjerite postojeće grupe iz [Office 365 iz centra za administraciju](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="cc50c-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="cc50c-109">Da biste riješili problem, izbrišite postojeću grupu ako više nije potrebna ili stvorite web-mjesto s dodijeljenim drugim pseudonimom.</span><span class="sxs-lookup"><span data-stu-id="cc50c-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="cc50c-110">Postoje različiti načini stvaranja i korištenja modernih grupa u sustavu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cc50c-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="cc50c-111">Postojeća web-mjesta možete povezati s Officeovom 365 grupom.</span><span class="sxs-lookup"><span data-stu-id="cc50c-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="cc50c-112">Dodatne informacije potražite [u okviru Povezivanje grupe sustava Office 365 pomoću web-mjesta korisnika sustava SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="cc50c-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="cc50c-113">Za stvaranje povezanog web-mjesta sustava Office 365, morat ćete stvoriti timsko web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="cc50c-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="cc50c-114">Dodatne informacije potražite [u okviru Stvaranje timskog web-mjesta u sustavu SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="cc50c-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

