---
title: 1491-pretraživanje-ne-vraća-očekuje-Rezultati
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740466"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="9180a-102">Pretraživanje sadržaja ne vraća očekivane rezultate</span><span class="sxs-lookup"><span data-stu-id="9180a-102">Content Search not returning expected results</span></span>

<span data-ttu-id="9180a-103">Kada pokrenete pretraživanje sadržaja iz centra za & sigurnost sustava Microsoft 365, možda će vam se prikazati neočekivan rezultat pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="9180a-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="9180a-104">Razmotrite sljedeće stavke koje mogu utjecati na rezultate pretraživanja:</span><span class="sxs-lookup"><span data-stu-id="9180a-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="9180a-105">**Mjesta sadržaja i uvjeti pretraživanja**: Provjerite jeste li odabrali odgovarajuće lokacije sadržaja i uvjete pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="9180a-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="9180a-106">Ako ste pokrenuli veliko pretraživanje (s mnogo mjesta), razmotrite njegovo razdvajanje u više pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="9180a-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="9180a-107">**Djelomično indeksirane stavke**:  [djelomično indeksirane stavke](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) iz poštanskih sandučića uvršteni su u procijenjene rezultate pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="9180a-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="9180a-108">Međutim, djelomično indeksirane stavke s web-mjesta u sustavu SharePoint i OneDrive nisu uključene u procjenu pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="9180a-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="9180a-109">Pogreške u **pretraživanju**: Kada pretražujete veliki broj poštanskih sandučića (iznad 100.000 poštanskih sandučića), možda će vam se prilikom pretraživanja pojavljuje pogreška u pretraživanju uz šifre pogrešaka kao što su CS008-009 i CS012-002).</span><span class="sxs-lookup"><span data-stu-id="9180a-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="9180a-110">U ovom slučaju ponovno pokušajte pretraživati samo za neuspjela mjesta sadržaja.</span><span class="sxs-lookup"><span data-stu-id="9180a-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="9180a-111">Dodatne informacije potražite u  [ovom članku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="9180a-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
