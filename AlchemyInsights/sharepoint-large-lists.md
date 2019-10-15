---
title: SharePoint veliki popisi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488509"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="4b0a0-102">Rad s velikim popisima i bibliotekama u sustavu SharePoint</span><span class="sxs-lookup"><span data-stu-id="4b0a0-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="4b0a0-103">SharePointovi popisi i biblioteke mogu sadržavati do 30.000.000 artikala, ali kada imaju više od 5.000 artikala, možda ćete vidjeti pogrešku praga prikaza popisa kada pokušate raditi s njima.</span><span class="sxs-lookup"><span data-stu-id="4b0a0-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="4b0a0-104">Ovaj prag je na mjestu za održavanje izvedbe usluge.</span><span class="sxs-lookup"><span data-stu-id="4b0a0-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="4b0a0-105">Ne može se promijeniti.</span><span class="sxs-lookup"><span data-stu-id="4b0a0-105">It can't be changed.</span></span> <span data-ttu-id="4b0a0-106">Da biste izbjegli udarni prag:</span><span class="sxs-lookup"><span data-stu-id="4b0a0-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="4b0a0-107">**Koristite moderne**</span><span class="sxs-lookup"><span data-stu-id="4b0a0-107">**Use modern**</span></span>

<span data-ttu-id="4b0a0-108">Prikazi koji prikazuju mnoge stavke najbolje rade u modernom iskustvu.</span><span class="sxs-lookup"><span data-stu-id="4b0a0-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="4b0a0-109">[Koristite moderno iskustvo](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) kako biste izbjegli pogreške koje biste mogli vidjeti u klasičnom iskustvu.</span><span class="sxs-lookup"><span data-stu-id="4b0a0-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="4b0a0-110">**Dodavanje indeksa**</span><span class="sxs-lookup"><span data-stu-id="4b0a0-110">**Add indexes**</span></span>

<span data-ttu-id="4b0a0-111">Kada filtrirate ili sortirati po stupcu koji nema indeks, možda ćete vidjeti poruku o pogrešci.</span><span class="sxs-lookup"><span data-stu-id="4b0a0-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="4b0a0-112">Ručno [dodajte indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) iz **postavki popisa** u izborniku postavki, a zatim **indeksirani stupci**.</span><span class="sxs-lookup"><span data-stu-id="4b0a0-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="4b0a0-113">**Uređivanje prikaza popisa**</span><span class="sxs-lookup"><span data-stu-id="4b0a0-113">**Edit the list view**</span></span>

<span data-ttu-id="4b0a0-114">Ako se pojavi pogreška pri radu s velikim popisom, [uredite prikaz popisa](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="4b0a0-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="4b0a0-115">Sljedeće četiri promjene uklonit će pogreške praga prikaza popisa.</span><span class="sxs-lookup"><span data-stu-id="4b0a0-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="4b0a0-116">Napravite sve četiri promjene kako biste uklonili sve pogreške.</span><span class="sxs-lookup"><span data-stu-id="4b0a0-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="4b0a0-117">Ako još uvijek dobijate pogreške, provjerite [Upravljanje velikim popisima i bibliotekama](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="4b0a0-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="4b0a0-118">Odaberite **ništa** iz oba **prvog sortiranja po stupcu** , a **zatim sortirajte po stupcu**.</span><span class="sxs-lookup"><span data-stu-id="4b0a0-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="4b0a0-119">Odaberite **ništa** iz obje **prve grupe po stupcu** , a **zatim grupirajte po stupcu**.</span><span class="sxs-lookup"><span data-stu-id="4b0a0-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="4b0a0-120">Odaberite **ništa** za sve stupce u sekciji **ukupnih zbrojeva** .</span><span class="sxs-lookup"><span data-stu-id="4b0a0-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="4b0a0-121">Poništite odabir svih osim jednog stupca za prikaz iz sekcije **Stupci** .</span><span class="sxs-lookup"><span data-stu-id="4b0a0-121">Deselect all but one column for display from the **Columns** section.</span></span>

