---
title: Smjernice za performanse opće migracije
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932471"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="84952-102">Smjernice za performanse opće migracije</span><span class="sxs-lookup"><span data-stu-id="84952-102">General migration performance guidance</span></span>

<span data-ttu-id="84952-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokreću poslovne ključne aplikacije na servis koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="84952-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="84952-104">To obuhvaća migraciju sadržaja, sprječavanje gubitka podataka (DLP) i rješenja za sigurnosno kopiranje.</span><span class="sxs-lookup"><span data-stu-id="84952-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="84952-105">Tijekom tih presedana poduzimamo korake da bi servisi sustava SharePoint Online i servisi OneDrive ostali iznimno raspoloživi i pouzdani za korisnike koji više nego ikad ovise o servisu u udaljenim radnim scenarijima.</span><span class="sxs-lookup"><span data-stu-id="84952-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="84952-106">Na temelju podrške tog cilja implementirali smo čvršća restriktivna ograničenja na pozadinske aplikacije (migracija, DLP i rješenja sigurnosnih kopija) tijekom radnog dana.</span><span class="sxs-lookup"><span data-stu-id="84952-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="84952-107">Trebali biste očekivati da će te aplikacije tijekom tog vremena doseći ograničen protok.</span><span class="sxs-lookup"><span data-stu-id="84952-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="84952-108">No tijekom večeri i vikenda u regiji servis će biti spreman za obradu znatno većeg volumena zahtjeva iz pozadinske aplikacije.</span><span class="sxs-lookup"><span data-stu-id="84952-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="84952-109">**Smjernice za performanse migracije**</span><span class="sxs-lookup"><span data-stu-id="84952-109">**Migration performance guidance**</span></span>

<span data-ttu-id="84952-110">Na performanse migracije mogu utjecati mrežna infrastruktura, veličina datoteke, vrijeme migracije te ograničavanje.</span><span class="sxs-lookup"><span data-stu-id="84952-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="84952-111">Razumijevanje gore navedenog olakšat će vam planiranje i maksimiziranje efikasnosti migracije.</span><span class="sxs-lookup"><span data-stu-id="84952-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="84952-112">Smjernice za performanse opće migracije</span><span class="sxs-lookup"><span data-stu-id="84952-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
