---
title: Očekivani rezultati za 1491-search-not-returning
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510564"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="23a8e-102">Pretraživanje sadržaja ne vraća očekivane rezultate</span><span class="sxs-lookup"><span data-stu-id="23a8e-102">Content Search not returning expected results</span></span>

<span data-ttu-id="23a8e-103">Prilikom pokretanja pretraživanja sadržaja iz centra za usklađenost & sustava Microsoft 365, možda ćete primiti neočekivane rezultate pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="23a8e-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="23a8e-104">Razmotrite sljedeće stvari koje mogu utjecati na rezultate pretraživanja:</span><span class="sxs-lookup"><span data-stu-id="23a8e-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="23a8e-105">**Lokacije sadržaja i uvjeti pretraživanja**: Provjerite jeste li odabrali odgovarajuće lokacije sadržaja i uvjete pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="23a8e-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="23a8e-106">Ako ste pokrenuli veliko pretraživanje (s mnogo lokacija), razmislite o tome da ga podijelite u više pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="23a8e-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="23a8e-107">**Djelomično indeksirane stavke**: [Djelomično indeksirane stavke](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) iz poštanskih sandučića uključene su u procijenjene rezultate pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="23a8e-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="23a8e-108">Međutim, djelomično indeksirane stavke s web-mjesta u sustavima SharePoint i OneDrive nisu uključene u procjenu pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="23a8e-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="23a8e-109">**Pogreške u pretraživanju**: prilikom pretraživanja velikog broja poštanskih sandučića (više od 100 000 poštanskih sandučića), možda ćete dobiti pogreške pretraživanja s kodovima pogrešaka kao što su CS008-009 i CS012-002).</span><span class="sxs-lookup"><span data-stu-id="23a8e-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="23a8e-110">U tom slučaju pokušajte potražiti samo za neuspjele lokacije sadržaja.</span><span class="sxs-lookup"><span data-stu-id="23a8e-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="23a8e-111">Dodatne informacije potražite u [ovom članku.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)</span><span class="sxs-lookup"><span data-stu-id="23a8e-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
