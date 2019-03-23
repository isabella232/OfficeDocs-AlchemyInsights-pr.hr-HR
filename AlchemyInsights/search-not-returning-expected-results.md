---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776074"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="a9b29-102">Sadržaja nije uputio očekivane rezultate pretraživanja</span><span class="sxs-lookup"><span data-stu-id="a9b29-102">Content Search not returning expected results</span></span>

<span data-ttu-id="a9b29-103">Prilikom izvođenja pretraživanja sadržaja iz & Office 365 Sigurnosni centar usklađenosti primiti neočekivani rezultati.</span><span class="sxs-lookup"><span data-stu-id="a9b29-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="a9b29-104">Razmotrite sljedeće stvari koje mogu utjecati na rezultate pretraživanja:</span><span class="sxs-lookup"><span data-stu-id="a9b29-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="a9b29-105">**Mjesta sadržaja i uvjete pretraživanja**: Provjerite ste odabrali odgovarajući mjesta sadržaja i uvjete pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="a9b29-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="a9b29-106">Ako ste pokrenuli veliki pretraživanja (s mnogih mjesta), razmislite o podjele u više pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="a9b29-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="a9b29-107">**Djelomično indeksirane stavke**: [djelomično indeksirane stavke](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) poštanske sandučiće su uključeni u rezultatima pretraživanja procijenjeni.</span><span class="sxs-lookup"><span data-stu-id="a9b29-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="a9b29-108">Međutim, djelomično indeksirane stavke s mjesta u SharePoint i OneDrive nisu uključeni u procjenu pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="a9b29-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="a9b29-109">**Pretraživanje neuspjeha**: prilikom pretraživanja velik broj poštanski sandučići (više od 100 000 poštanske sandučiće), možda ćete dobiti pogreške pretraživanja s kodovi pogreške kao što su CS008 009 i CS012 002).</span><span class="sxs-lookup"><span data-stu-id="a9b29-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="a9b29-110">U tom slučaju, ponovno pretraživanje samo za mjesta sadržaja nije uspjelo.</span><span class="sxs-lookup"><span data-stu-id="a9b29-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="a9b29-111">Pogledajte [Ovaj članak](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) dodatne informacije.</span><span class="sxs-lookup"><span data-stu-id="a9b29-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
