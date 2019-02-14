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
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964821"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="3efc5-102">Sadržaja nije uputio očekivane rezultate pretraživanja</span><span class="sxs-lookup"><span data-stu-id="3efc5-102">Content Search not returning expected results</span></span>

<span data-ttu-id="3efc5-p101">Prilikom izvođenja pretraživanja sadržaja iz & Office 365 Sigurnosni centar usklađenosti primiti neočekivani rezultati. Razmotrite sljedeće stvari koje mogu utjecati na rezultate pretraživanja:</span><span class="sxs-lookup"><span data-stu-id="3efc5-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="3efc5-p102">**Mjesta sadržaja i uvjete pretraživanja**: Provjerite ste odabrali odgovarajući mjesta sadržaja i uvjete pretraživanja. Ako ste pokrenuli veliki pretraživanja (s mnogih mjesta), razmislite o podjele u više pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="3efc5-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="3efc5-p103">**Djelomično indeksirane stavke**: [djelomično indeksirane stavke](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) poštanske sandučiće su uključeni u rezultatima pretraživanja procijenjeni. Međutim, djelomično indeksirane stavke s mjesta u SharePoint i OneDrive nisu uključeni u procjenu pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="3efc5-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="3efc5-p104">**Pretraživanje neuspjeha**: prilikom pretraživanja velik broj poštanski sandučići (više od 100 000 poštanske sandučiće), možda ćete dobiti pogreške pretraživanja s kodovi pogreške kao što su CS008 009 i CS012 002). U tom slučaju, ponovno pretraživanje samo za mjesta sadržaja nije uspjelo. Pogledajte [Ovaj članak](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) dodatne informacije.</span><span class="sxs-lookup"><span data-stu-id="3efc5-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
