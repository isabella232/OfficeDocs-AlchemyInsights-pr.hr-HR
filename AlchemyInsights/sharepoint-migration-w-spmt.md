---
title: Migracija sustava SharePoint sa SPMT-om
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931542"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="64d39-102">Migracija sustava SharePoint sa SPMT-om</span><span class="sxs-lookup"><span data-stu-id="64d39-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="64d39-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="64d39-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="64d39-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="64d39-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="64d39-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="64d39-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="64d39-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="64d39-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="64d39-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="64d39-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="64d39-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="64d39-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="64d39-109">**Alat za migraciju sustava SharePoint**</span><span class="sxs-lookup"><span data-stu-id="64d39-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="64d39-110">Dizajniran za migracije u rasponu od najmanjeg skupa datoteka do migracije poduzeća velikih razmjera, alat za migraciju sustava SharePoint omogućit će vam prijenos podataka u oblak i iskorištavanje najnovije suradnje, inteligencije i sigurnosna rješenja u sustavu Office 365.</span><span class="sxs-lookup"><span data-stu-id="64d39-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="64d39-111">Preuzimanje i instalacija alata za migraciju sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="64d39-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="64d39-112">Otklanjanje uobičajenih Problema s APMT-om i pogreškama</span><span class="sxs-lookup"><span data-stu-id="64d39-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="64d39-113">Otklanjanje poteškoća s instalacijom SPMT-a</span><span class="sxs-lookup"><span data-stu-id="64d39-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
