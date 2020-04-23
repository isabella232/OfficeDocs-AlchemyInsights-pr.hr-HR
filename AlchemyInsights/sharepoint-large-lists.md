---
title: Veliki popisi sustava SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767277"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="33e7b-102">Rad s velikim popisima i bibliotekama u sustavu SharePoint</span><span class="sxs-lookup"><span data-stu-id="33e7b-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="33e7b-103">Popisi i biblioteke sustava SharePoint mogu sadržavati do 30 milijuna stavki, ali kada imaju više od 5000 stavki, možda ćete vidjeti pogrešku praga prikaza popisa kada pokušate raditi s njima.</span><span class="sxs-lookup"><span data-stu-id="33e7b-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="33e7b-104">Prag je postavljen radi zadržavanja performansi servisa.</span><span class="sxs-lookup"><span data-stu-id="33e7b-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="33e7b-105">Nije ga moguće promijeniti.</span><span class="sxs-lookup"><span data-stu-id="33e7b-105">It can't be changed.</span></span> <span data-ttu-id="33e7b-106">Da biste izbjegli udaranje tog praga:</span><span class="sxs-lookup"><span data-stu-id="33e7b-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="33e7b-107">**Koristite moderne**</span><span class="sxs-lookup"><span data-stu-id="33e7b-107">**Use modern**</span></span>

<span data-ttu-id="33e7b-108">Prikazi koji prikazuju mnoge stavke najbolje funkcioniraju u modernom doživljaju.</span><span class="sxs-lookup"><span data-stu-id="33e7b-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="33e7b-109">[Koristite suvremeni doživljaj](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) da biste izbjegli pogreške koje biste mogli vidjeti u klasičnom doživljaju.</span><span class="sxs-lookup"><span data-stu-id="33e7b-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="33e7b-110">**Dodavanje indeksa**</span><span class="sxs-lookup"><span data-stu-id="33e7b-110">**Add indexes**</span></span>

<span data-ttu-id="33e7b-111">Kada filtrirate ili sortirate po stupcu koji nema indeks, možda će vam se prikazati poruka o pogrešci.</span><span class="sxs-lookup"><span data-stu-id="33e7b-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="33e7b-112">[Ručno dodajte indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) iz **postavki popisa** u izborniku postavki, a zatim **Indeksirani stupci**.</span><span class="sxs-lookup"><span data-stu-id="33e7b-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="33e7b-113">**Uređivanje prikaza popisa**</span><span class="sxs-lookup"><span data-stu-id="33e7b-113">**Edit the list view**</span></span>

<span data-ttu-id="33e7b-114">Ako dođe do pogreške prilikom rada s velikim popisom, [uredite prikaz popisa](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="33e7b-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="33e7b-115">Sljedeće četiri promjene uklonit će pogreške praga prikaza popisa.</span><span class="sxs-lookup"><span data-stu-id="33e7b-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="33e7b-116">Napravite sve četiri promjene da biste uklonili sve pogreške.</span><span class="sxs-lookup"><span data-stu-id="33e7b-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="33e7b-117">Ako i dalje primate pogreške, provjerite [Upravljanje velikim popisima i bibliotekama](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="33e7b-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="33e7b-118">Odaberite **Ništa** iz oba **Prvo sortiranje po stupcu** i **Zatim sortirajte po stupcu**.</span><span class="sxs-lookup"><span data-stu-id="33e7b-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="33e7b-119">Odaberite **Ništa** iz obje **grupe Prvi po stupcu** i **Zatim grupirajte po stupcu**.</span><span class="sxs-lookup"><span data-stu-id="33e7b-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="33e7b-120">Odaberite **Ništa** za sve stupce u odjeljku **Ukupni zbrojevi.**</span><span class="sxs-lookup"><span data-stu-id="33e7b-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="33e7b-121">Poništite odabir svih osim jednog stupca za prikaz iz **odjeljka Stupci.**</span><span class="sxs-lookup"><span data-stu-id="33e7b-121">Deselect all but one column for display from the **Columns** section.</span></span>

