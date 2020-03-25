---
title: Otklanjanje poteškoća s alatom za migraciju sustava SharePoint i pogreškama
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931110"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="2f8cf-102">Otklanjanje poteškoća s alatom za migraciju sustava SharePoint i pogreškama</span><span class="sxs-lookup"><span data-stu-id="2f8cf-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="2f8cf-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="2f8cf-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2f8cf-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="2f8cf-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2f8cf-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="2f8cf-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2f8cf-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="2f8cf-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2f8cf-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="2f8cf-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2f8cf-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="2f8cf-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2f8cf-109">**Uobičajeni problemi i pogreške**</span><span class="sxs-lookup"><span data-stu-id="2f8cf-109">**Common issues and errors**</span></span>

<span data-ttu-id="2f8cf-110">Prilikom korištenja alata za migraciju sustava SharePoint (SPMT) možete naići na neke uobičajene probleme i pogreške.</span><span class="sxs-lookup"><span data-stu-id="2f8cf-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="2f8cf-111">Dodatne informacije potražite na vezama u nastavku.</span><span class="sxs-lookup"><span data-stu-id="2f8cf-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="2f8cf-112">Otklanjanje uobičajenih Problema s APMT-om i pogreškama</span><span class="sxs-lookup"><span data-stu-id="2f8cf-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="2f8cf-113">Otklanjanje poteškoća s instalacijom SPMT-a</span><span class="sxs-lookup"><span data-stu-id="2f8cf-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)