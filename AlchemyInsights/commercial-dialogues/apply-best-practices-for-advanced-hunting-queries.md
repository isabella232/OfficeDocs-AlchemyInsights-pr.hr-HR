---
title: Primjena najboljih postupaka za napredne lovačke upite
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743704"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="e559a-102">Primjena najboljih postupaka za napredne lovačke upite</span><span class="sxs-lookup"><span data-stu-id="e559a-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="e559a-103">Da biste ubrzali rezultate i izbjegli vremenske korake tijekom izvođenja složenih upita, primijenite ove najbolje prakse:</span><span class="sxs-lookup"><span data-stu-id="e559a-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="e559a-104">Prilikom pokušaja novih upita uvijek koristite ograničenje da biste izbjegli krajnje velike skupove rezultata.</span><span class="sxs-lookup"><span data-stu-id="e559a-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="e559a-105">Upotrijebite i `count` da biste postavili početnu ocjenu veličine skupa rezultata.</span><span class="sxs-lookup"><span data-stu-id="e559a-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="e559a-106">Najprije koristite filtre vremena.</span><span class="sxs-lookup"><span data-stu-id="e559a-106">Use time filters first.</span></span> <span data-ttu-id="e559a-107">U idealno, ograničite upite na sedam dana.</span><span class="sxs-lookup"><span data-stu-id="e559a-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="e559a-108">Na početku upita odmah nakon filtra vremena Dodajte filtre za koje se očekuje da će ukloniti većinu podataka.</span><span class="sxs-lookup"><span data-stu-id="e559a-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="e559a-109">Kada tražite pune žetone, koristite operator, `has` a ne `contains` .</span><span class="sxs-lookup"><span data-stu-id="e559a-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="e559a-110">Pokrenite pretraživanje na određenom stupcu, a ne u svim stupcima.</span><span class="sxs-lookup"><span data-stu-id="e559a-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="e559a-111">Kada se pridružite tablicama, najprije navedite tablicu s manje redaka.</span><span class="sxs-lookup"><span data-stu-id="e559a-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="e559a-112">`project` Samo potrebne stupce iz tablica kojima ste se pridružili.</span><span class="sxs-lookup"><span data-stu-id="e559a-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="e559a-113">Dodatne informacije potražite u članku [najbolje prakse za napredne lovačke upite](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="e559a-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
