---
title: Veliki popisi sustava SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720125"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="6af57-102">Rad s velikim popisima i bibliotekama u sustavu SharePoint</span><span class="sxs-lookup"><span data-stu-id="6af57-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="6af57-103">Popisi i biblioteke sustava SharePoint mogu sadržavati do 30.000.000 stavki, ali kada imaju više od 5.000 stavki, možda će vam se prikazati pogreška praga prikaza popisa kada pokušate raditi s njima.</span><span class="sxs-lookup"><span data-stu-id="6af57-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="6af57-104">Prag je postavljen radi zadržavanja performansi servisa.</span><span class="sxs-lookup"><span data-stu-id="6af57-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="6af57-105">Nije ga moguće promijeniti.</span><span class="sxs-lookup"><span data-stu-id="6af57-105">It can't be changed.</span></span> <span data-ttu-id="6af57-106">Da biste izbjegli udarajući Prag, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="6af57-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="6af57-107">**Koristite moderne**</span><span class="sxs-lookup"><span data-stu-id="6af57-107">**Use modern**</span></span>

<span data-ttu-id="6af57-108">Prikazi koji prikazuju mnoge stavke najbolje funkcioniraju u modernom iskustvu.</span><span class="sxs-lookup"><span data-stu-id="6af57-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="6af57-109">[Koristite moderno iskustvo](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) da biste izbjegli pogreške koje biste mogli vidjeti u klasičnom iskustvu.</span><span class="sxs-lookup"><span data-stu-id="6af57-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="6af57-110">**Dodavanje indeksa**</span><span class="sxs-lookup"><span data-stu-id="6af57-110">**Add indexes**</span></span>

<span data-ttu-id="6af57-111">Kada filtrirate ili sortirate prema stupcu koji nema indeks, možda će vam se prikazati poruka o pogrešci.</span><span class="sxs-lookup"><span data-stu-id="6af57-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="6af57-112">Ručno [dodajte indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) iz **postavki popisa** na izborniku Postavke, a zatim **indeksirani stupci**.</span><span class="sxs-lookup"><span data-stu-id="6af57-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="6af57-113">**Uređivanje prikaza popisa**</span><span class="sxs-lookup"><span data-stu-id="6af57-113">**Edit the list view**</span></span>

<span data-ttu-id="6af57-114">Ako se pojavi pogreška prilikom rada s velikim popisom, [uredite prikaz popisa](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="6af57-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="6af57-115">Sljedeće četiri promjene uklonit će pogreške praga prikaza popisa.</span><span class="sxs-lookup"><span data-stu-id="6af57-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="6af57-116">Izvršite sve četiri promjene da biste uklonili sve pogreške.</span><span class="sxs-lookup"><span data-stu-id="6af57-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="6af57-117">Ako i dalje dobivate pogreške, provjerite [Upravljanje velikim popisima i bibliotekama](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="6af57-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="6af57-118">Odaberite **ništa** od **prvog sortiranja prema stupcu** , a **zatim sortirajte po stupcu**.</span><span class="sxs-lookup"><span data-stu-id="6af57-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="6af57-119">Odaberite **nema** iz **prve grupe prema stupcu** , a **zatim Grupiraj prema stupcu**.</span><span class="sxs-lookup"><span data-stu-id="6af57-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="6af57-120">Odaberite **nema** za sve stupce u odjeljku **Ukupni zbrojevi** .</span><span class="sxs-lookup"><span data-stu-id="6af57-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="6af57-121">Poništite odabir svih stupaca, no jedan za prikaz iz sekcije **Stupci** .</span><span class="sxs-lookup"><span data-stu-id="6af57-121">Deselect all but one column for display from the **Columns** section.</span></span>

