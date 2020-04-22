---
title: 1491-search-not-returning-očekivani rezultati
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
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709219"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="d5618-102">Pretraživanje sadržaja ne vraća očekivane rezultate</span><span class="sxs-lookup"><span data-stu-id="d5618-102">Content Search not returning expected results</span></span>

<span data-ttu-id="d5618-103">Prilikom pokretanja pretraživanja sadržaja iz centra za sigurnost sustava Microsoft 365 & centru za usklađenost, možda ćete dobiti neočekivane rezultate pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="d5618-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="d5618-104">Razmotrite sljedeće stvari koje mogu utjecati na rezultate pretraživanja:</span><span class="sxs-lookup"><span data-stu-id="d5618-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="d5618-105">**Lokacije sadržaja i uvjeti pretraživanja:** Provjerite jeste li odabrali odgovarajuće lokacije sadržaja i uvjete pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="d5618-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="d5618-106">Ako ste pokrenuli veliko pretraživanje (s mnogo lokacija), razmislite o podjeli u više pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="d5618-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="d5618-107">**Djelomično indeksirane stavke**: [Djelomično indeksirane stavke](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) iz poštanskih sandučića uključene su u procijenjene rezultate pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="d5618-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="d5618-108">Međutim, djelomično indeksirane stavke s web-mjesta u sustavu SharePoint i OneDrive nisu uključene u procjenu pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="d5618-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="d5618-109">**Pogreške u pretraživanju**: Prilikom pretraživanja velikog broja poštanskih sandučića (više od 100 000 poštanskih sandučića) možete dobiti pogreške pretraživanja s kodovima pogrešaka kao što su CS008-009 i CS012-002).</span><span class="sxs-lookup"><span data-stu-id="d5618-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="d5618-110">U tom slučaju ponovno pokušajte pretraživati samo za neuspjela mjesta sadržaja.</span><span class="sxs-lookup"><span data-stu-id="d5618-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="d5618-111">Dodatne informacije potražite [u ovom članku.](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)</span><span class="sxs-lookup"><span data-stu-id="d5618-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
