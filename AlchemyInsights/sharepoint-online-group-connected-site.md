---
title: Dodavanje grupe web-mjesta sustava SharePoint
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
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750512"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="7c449-102">Problemi kada stvaranja ili grupe povezani web-mjesta u SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7c449-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="7c449-103">Postoji nekoliko uobičajenih problema naišao je na prilikom stvaranja ili ponovno stvaranje grupe povezani web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="7c449-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="7c449-104">Ako ste izbrisali grupu i njegovih povezanih web-mjesta i želite stvoriti drugu web-mjesta s istim URL, morat ćete trajno ukloniti prethodno web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="7c449-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="7c449-105">Preuzimanje [SPO upravljanja ljuske](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="7c449-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="7c449-106">Dodatne informacije na Uvod powershell potražite [Uvod u SharePoint Online ljuske za upravljanje](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="7c449-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="7c449-107">Uklanjanje web-mjesta iz izbrisane web-mjesta pomoću cmdleta [Ukloni-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell.</span><span class="sxs-lookup"><span data-stu-id="7c449-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="7c449-108">Ako izradi grupe povezanih web-mjesta i primiti upozorenje drugu grupu s iste alias već postoji, provjerite postojeće grupe iz [centra za administraciju sistema Office 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="7c449-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="7c449-109">Da biste riješili taj problem, izbrišite postojeće grupe ako više nije potrebna ili stvaranje web-mjesta s različitim Pseudonim dodijeljen.</span><span class="sxs-lookup"><span data-stu-id="7c449-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="7c449-110">Stvaranje i korištenje Moderna grupe s SharePoint na različite načina.</span><span class="sxs-lookup"><span data-stu-id="7c449-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="7c449-111">Postojeća web-mjesta možete se povezati s Office 365 grupe.</span><span class="sxs-lookup"><span data-stu-id="7c449-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="7c449-112">Za dodatne informacije pogledajte [povezivanje programa Office 365 grupu pomoću ineterface korisnika SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="7c449-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="7c449-113">Da biste stvorili programa Office 365 grupe povezanih web-mjesta, trebat ćete stvoriti web-mjesto tima.</span><span class="sxs-lookup"><span data-stu-id="7c449-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="7c449-114">Dodatne informacije potražite u članku [Kreiranje web-mjesto tima u SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="7c449-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

