---
title: Ograničavanje migracije sustava SharePoint s 503 pogreške
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931650"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="c4b8e-102">Ograničavanje migracije sustava SharePoint s 503 pogreške</span><span class="sxs-lookup"><span data-stu-id="c4b8e-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="c4b8e-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c4b8e-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c4b8e-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c4b8e-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c4b8e-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c4b8e-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c4b8e-109">**503 pogreške prilikom migracije u SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="c4b8e-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="c4b8e-110">Čini se da migrirate u SharePoint Online i primate 503 pogreške.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="c4b8e-111">Slijedite korake u nastavku kako bismo vam mogli pomoći što je prije moguće.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="c4b8e-112">Kliknite **Obratite se službi za podršku**, a zatim Novi zahtjev za **servisom**.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="c4b8e-113">Za naslov i opis upišite **Ograničavanje migracije sustava SharePoint s 503**.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="c4b8e-114">Nakon podnošenja karte ažurirajte je sljedećim informacijama:</span><span class="sxs-lookup"><span data-stu-id="c4b8e-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="c4b8e-115">Koliko je ostalo migracije (na primjer, koliko tbs?).</span><span class="sxs-lookup"><span data-stu-id="c4b8e-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="c4b8e-116">Datum početka i završetka migracije.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-116">Migration start and end date.</span></span>
    - <span data-ttu-id="c4b8e-117">Opišite odakle migrirate sadržaj, kao što su SharePoint Server, Box, GDrive, Zajedničko korištenje datoteka itd..</span><span class="sxs-lookup"><span data-stu-id="c4b8e-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="c4b8e-118">Procijeniti broj pogrešaka regulacije (na primjer, x gasa na sat?) i kada se regulacija dogodila.</span><span class="sxs-lookup"><span data-stu-id="c4b8e-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="c4b8e-119">Koji alat za migraciju koristite (na primjer, SPMT ili ShareGate).</span><span class="sxs-lookup"><span data-stu-id="c4b8e-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


