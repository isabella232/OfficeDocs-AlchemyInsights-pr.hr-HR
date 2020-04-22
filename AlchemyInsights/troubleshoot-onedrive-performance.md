---
title: Otklanjanje poteškoća s performansama servisa OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 197a84c5f69f9e58460925049345263743fe78ee
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43733190"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="943c8-102">Otklanjanje poteškoća s performansama servisa OneDrive</span><span class="sxs-lookup"><span data-stu-id="943c8-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="943c8-103">Ako imate sporiji od očekivane sinkronizacije ili probleme sa sličnim performansama sa servisom OneDrive:</span><span class="sxs-lookup"><span data-stu-id="943c8-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="943c8-104">Potvrdite da nema poznatih problema pomoću [nadzorne ploče stanja servisa](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="943c8-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="943c8-105">[Omogućite datoteke na zahtjev](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) da biste svim datotekama na servisu OneDrive mogli pristupiti bez potrebe za preuzimanjem svih datoteka i korištenjem prostora za pohranu na uređaju.</span><span class="sxs-lookup"><span data-stu-id="943c8-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="943c8-106">[Pregledajte najbolje primjere iz prakse](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) za planiranje i performanse mreže.</span><span class="sxs-lookup"><span data-stu-id="943c8-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="943c8-107">[Maksimizirajte brzinu prijenosa i preuzimanja,](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)osobito ako sinkronizirate uređaj prvi put.</span><span class="sxs-lookup"><span data-stu-id="943c8-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="943c8-108">Ako sinkronizirate biblioteku s više od 100 000 stavki, sinkronizacija servisa OneDrive može se dugo prikazivati ili status prikazuje obradu 0KB xMB-a."</span><span class="sxs-lookup"><span data-stu-id="943c8-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="943c8-109">[Saznajte više o sinkronizaciji više od 100.000 datoteka](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) kao i [podržanog ograničenja od 300 000 datoteka na servisu OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="943c8-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="943c8-110">Kada korisnik premaši ograničenja korištenja, SharePoint Online zamrači sve dodatne zahtjeve s tog korisničkog računa na kratko razdoblje.</span><span class="sxs-lookup"><span data-stu-id="943c8-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="943c8-111">Sve akcije korisnika su gasite dok je gas na snazi.</span><span class="sxs-lookup"><span data-stu-id="943c8-111">All user actions are throttled while the throttle is in effect.</span></span>
