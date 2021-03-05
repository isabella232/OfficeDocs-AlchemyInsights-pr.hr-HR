---
title: Izvoz rezultata pretraživanja Iotkrivanja i sadržaja
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481281"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="16b75-102">Izvoz rezultata pretraživanja Iotkrivanja i sadržaja</span><span class="sxs-lookup"><span data-stu-id="16b75-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="16b75-103">Možda ćete morati izvoziti rezultate pretraživanja u PST datoteku (iz e-pošte) ili na izvorne dokumente sustava Office (sa web-mjesta sustava SharePoint i servisa OneDrive za tvrtke).</span><span class="sxs-lookup"><span data-stu-id="16b75-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="16b75-104">Ako je tako, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="16b75-104">If so, do the following:</span></span>

- <span data-ttu-id="16b75-105">Provjerite je li vašem računu dodijeljeno odgovarajuće dozvole za izvoz.</span><span class="sxs-lookup"><span data-stu-id="16b75-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="16b75-106">Dodatne informacije potražite u članku [Dodjela dozvola za otkriće](https://go.microsoft.com/fwlink/?linkid=2102406).</span><span class="sxs-lookup"><span data-stu-id="16b75-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="16b75-107">Provjerite je li računalo zadovoljilo sve [preduvjete](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="16b75-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="16b75-108">Nisu podržani Svi preglednici, kao što je Chrome.</span><span class="sxs-lookup"><span data-stu-id="16b75-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="16b75-109">Da biste izvezli iz pretraživanja sadržaja: a.</span><span class="sxs-lookup"><span data-stu-id="16b75-109">To export from a Content Search: a.</span></span> <span data-ttu-id="16b75-110">Otvorite centar za [sigurnosnu &](https://protection.office.com/contentsearch) i kliknite **Pretraživanje**, a zatim odaberite **Pretraživanje sadržaja**.</span><span class="sxs-lookup"><span data-stu-id="16b75-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="16b75-111">Na stranici **Pretraživanje sadržaja** odaberite spremljeno pretraživanje.</span><span class="sxs-lookup"><span data-stu-id="16b75-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="16b75-112">b.</span><span class="sxs-lookup"><span data-stu-id="16b75-112">b.</span></span> <span data-ttu-id="16b75-113">U oknu s detaljima u odjeljku **Izvoz rezultata na računalo** odaberite **Započni izvoz**.</span><span class="sxs-lookup"><span data-stu-id="16b75-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="16b75-114">Ako izvozite više od 100K poštanskih sandučića, morat ćete koristiti PowerShell da biste preuzeli rezultate izvoza.</span><span class="sxs-lookup"><span data-stu-id="16b75-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="16b75-115">Dodatne informacije potražite u članku [Izvoz rezultata iz više od 100K poštanskih sandučića](https://go.microsoft.com/fwlink/?linkid=2143861).</span><span class="sxs-lookup"><span data-stu-id="16b75-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="16b75-116">Dodatne informacije potražite u članku [Izvoz rezultata pretraživanja sadržaja](https://go.microsoft.com/fwlink/?linkid=2102118).</span><span class="sxs-lookup"><span data-stu-id="16b75-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>