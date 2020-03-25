---
title: Problemi prilikom migracije podataka u SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931686"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="c3199-102">Problemi prilikom migracije podataka u SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c3199-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="c3199-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="c3199-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c3199-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="c3199-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c3199-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="c3199-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c3199-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="c3199-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c3199-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="c3199-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c3199-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="c3199-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c3199-109">**Migracija više od 100TB podataka**</span><span class="sxs-lookup"><span data-stu-id="c3199-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="c3199-110">Čini se da migrirate više od 100TB podataka u SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c3199-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="c3199-111">Slijedite korake u nastavku kako bismo vam mogli pomoći što je prije moguće.</span><span class="sxs-lookup"><span data-stu-id="c3199-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="c3199-112">Odaberite **Novi zahtjev za uslugom**, a zatim Novi zahtjev za **uslugom**.</span><span class="sxs-lookup"><span data-stu-id="c3199-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="c3199-113">Ostavite naslov i opis kao **migraciju sustava SharePoint preko 100TB**.</span><span class="sxs-lookup"><span data-stu-id="c3199-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="c3199-114">Nakon podnošenja karte ažurirajte je sljedećim informacijama:</span><span class="sxs-lookup"><span data-stu-id="c3199-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="c3199-115">Procijenjena veličina migracije.</span><span class="sxs-lookup"><span data-stu-id="c3199-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="c3199-116">Procjena o tome kada želite započeti i dovršiti migraciju.</span><span class="sxs-lookup"><span data-stu-id="c3199-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="c3199-117">Opišite odakle migrirate sadržaj, kao što su SharePoint Server, Box, GDrive, Zajedničko korištenje datoteka itd..</span><span class="sxs-lookup"><span data-stu-id="c3199-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

