---
title: Otklanjanje poteškoća s performansama servisa OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757877"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="8dfe6-102">Otklanjanje poteškoća s performansama servisa OneDrive</span><span class="sxs-lookup"><span data-stu-id="8dfe6-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="8dfe6-103">Ako nailazite na sporije od očekivane sinkronizacije ili slične poteškoće s performansama sa servisom OneDrive:</span><span class="sxs-lookup"><span data-stu-id="8dfe6-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="8dfe6-104">Potvrdite da nema poznatih problema pomoću [nadzorne ploče zdravstvene usluge](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8dfe6-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="8dfe6-105">[Omogućite datoteke na zahtjev](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) da biste mogli pristupiti svim datotekama na servisu OneDrive bez preuzimanja svih njih i korištenja prostora za pohranu na uređaju.</span><span class="sxs-lookup"><span data-stu-id="8dfe6-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="8dfe6-106">[Pregledajte najbolje prakse](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) za planiranje i performanse mreže.</span><span class="sxs-lookup"><span data-stu-id="8dfe6-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="8dfe6-107">[Maksimiziranje prijenosa i preuzimanja brzine](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), osobito ako prvi put sinkronizirate uređaj.</span><span class="sxs-lookup"><span data-stu-id="8dfe6-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="8dfe6-108">Ako sinkronizirate biblioteku s više od 100.000 stavki, Sinkronizacija servisa OneDrive može se učiniti dugo vremena ili status prikazuje obradu 0KB xMB. "</span><span class="sxs-lookup"><span data-stu-id="8dfe6-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="8dfe6-109">[Saznajte više o sinkronizaciji više od 100.000 datoteka](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , kao i [podržano ograničenje servisa OneDrive za 300.000 datoteka](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="8dfe6-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="8dfe6-110">Kada korisnik prelazi ograničenja korištenja, sustav SharePoint Online ograničit će daljnje zahtjeve s tog korisničkog računa u kratkom periodu.</span><span class="sxs-lookup"><span data-stu-id="8dfe6-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="8dfe6-111">Sve se korisničke akcije ograničuju dok je ventil na snazi.</span><span class="sxs-lookup"><span data-stu-id="8dfe6-111">All user actions are throttled while the throttle is in effect.</span></span>
