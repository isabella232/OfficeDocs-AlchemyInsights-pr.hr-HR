---
title: Otklanjanje poteškoća s problemima „Otvori pomoću programa Explorer” u programu SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6462"
- "9003546"
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ea93bb6f3cbbc3424f5e006ffac482a7445c8164
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086040"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="87a2d-102">Otklanjanje poteškoća s problemima „Otvori pomoću programa Explorer” u programu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="87a2d-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="87a2d-103">Slijedite korake i najbolje prakse u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="87a2d-103">Follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="87a2d-104">Korištenje naredbe „Otvori pomoću programa Explorer” za otklanjanje poteškoća u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="87a2d-104">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="87a2d-105">Kopiranje i premještanje datoteka biblioteke pomoću naredbe Otvori pomoću programa Explorer</span><span class="sxs-lookup"><span data-stu-id="87a2d-105">Copy or move library files by using Open with Explorer</span></span>](https://support.microsoft.com/office/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2?ui=en-us&rs=en-us&ad=us)

> [!NOTE]
- <span data-ttu-id="87a2d-106">Preporučujemo [sinkronizaciju datoteka sustava SharePoint s novim klijentom za sinkronizaciju servisa OneDrive](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) koji sadrži [datoteke na zahtjev](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) jer sinkronizacija dodjeljuje lokalni pristup datotekama i nudi najbolje performanse.</span><span class="sxs-lookup"><span data-stu-id="87a2d-106">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) which provides [Files On-Demand](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) because the synchronization grants local access to your files and offers the best performance.</span></span>

- <span data-ttu-id="87a2d-107">**Open with Explorer** podržan je samo u pregledniku Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="87a2d-107">**Open with Explorer** is only supported in Internet Explorer 11.</span></span> <span data-ttu-id="87a2d-108">Dodatne informacije potražite u članku [kraj podrške za IE 11 s aplikacijama Microsoft 365](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span><span class="sxs-lookup"><span data-stu-id="87a2d-108">For more information, see [end of support for IE11 with Microsoft 365 Apps](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span></span> <span data-ttu-id="87a2d-109">**Otvorite programom Explorer** ne funkcionira u sustavu Windows uz Microsoft Edge, Google Chrome, Mozilla Firefox ili na platformi Mac.</span><span class="sxs-lookup"><span data-stu-id="87a2d-109">**Open with Explorer** doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="87a2d-110">Zbog tog razloga mogućnost **prikaza eksplorera** može biti zasivljena.</span><span class="sxs-lookup"><span data-stu-id="87a2d-110">Due to this reason, the **Explorer View** option may be grayed out.</span></span> 

- <span data-ttu-id="87a2d-111">Gumb **Otvori pomoću programa Explorer** ne prikazuje se u novom doživljaju biblioteke.</span><span class="sxs-lookup"><span data-stu-id="87a2d-111">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="87a2d-112">Kliknite padajući izbornik **Prikaz** u gornjem desnom kutu (naziv padajućeg izbornika mijenja se ovisno o trenutnom prikazu), a zatim kliknite **Prikaži u eksploreru za datoteke**.</span><span class="sxs-lookup"><span data-stu-id="87a2d-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

