---
title: Otklanjanje poteškoća s problemima „Otvori pomoću programa Explorer” u programu SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 13149d288336b487441c66521b32406e408911fd
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35803030"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="25d47-102">Otklanjanje poteškoća s problemima „Otvori pomoću programa Explorer” u programu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="25d47-102">Troubleshoot “Open with Explorer” issues in Sharepoint Online</span></span>

<span data-ttu-id="25d47-103">Naredba Otvori pomoću programa Explorer otvara lokalnu instancu programa Windows Explorer koja prikazuje strukturu mapa na poslužitelju na kojem se nalazi web-mjesto sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="25d47-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="25d47-104">Ipak, preporučujemo [sinkronizaciju datoteka sustava SharePoint s novim klijentom za sinkronizaciju servisa OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, koji nudi [datoteke na zahtjev](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) jer to omogućuje lokalni pristup datotekama i nudi najbolje performanse.</span><span class="sxs-lookup"><span data-stu-id="25d47-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="25d47-105">Ako umjesto korištenja novog klijenta za sinkronizaciju servisa OneDrive odaberete korištenje prikaza u programu Explorer, pazite da slijedite korake i najbolje prakse iz prethodno navedenih članaka:</span><span class="sxs-lookup"><span data-stu-id="25d47-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="25d47-106">Korištenje naredbe „Otvori pomoću programa Explorer” za otklanjanje poteškoća u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="25d47-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="25d47-107">Kopiranje i premještanje datoteka biblioteke pomoću naredbe Otvori pomoću programa Explorer</span><span class="sxs-lookup"><span data-stu-id="25d47-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="25d47-108">Gumb **Otvori pomoću programa Explorer** ne prikazuje se u novom doživljaju biblioteke.</span><span class="sxs-lookup"><span data-stu-id="25d47-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="25d47-109">Kliknite padajući izbornik **Prikaz** u gornjem desnom kutu (naziv padajućeg izbornika mijenja se ovisno o trenutnom prikazu), a zatim kliknite **Prikaži u eksploreru za datoteke**.</span><span class="sxs-lookup"><span data-stu-id="25d47-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

 ><span data-ttu-id="25d47-110">Naredba Otvori pomoću programa Explorer u sustavu SharePoint koristi ActiveX kontrole pa je podržana samo u pregledniku Internet Explorer 10 ili 11.</span><span class="sxs-lookup"><span data-stu-id="25d47-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="25d47-111">Otvaranje pomoću programa Explorer ne funkcionira u sustavu Windows s preglednicima Microsoft Edge, Google Chrome, Mozilla Firefox ili na Mac platformi.</span><span class="sxs-lookup"><span data-stu-id="25d47-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="25d47-112">Zbog toga mogućnost Prikaz pretraživača može biti zasivljena.</span><span class="sxs-lookup"><span data-stu-id="25d47-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

> - <span data-ttu-id="25d47-113">[Zašto su gumbi vrpce sustava SharePoint nedostupni ili zasivljeni](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="25d47-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

