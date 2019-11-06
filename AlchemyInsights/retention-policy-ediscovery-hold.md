---
title: 2609-zadržavanje ili otkrivanje podataka-držite
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994050"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="89674-102">Nije moguće izbrisati stavke u SharePoint Online ili OneDrive za tvrtke</span><span class="sxs-lookup"><span data-stu-id="89674-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="89674-103">Vi ili vaši korisnici možda nećete moći izbrisati stavke u sustavu SharePoint Online ili OneDrive za tvrtke jer se pravila zadržavanja, oznaka zadržavanja ili zadržavanje dokumenata za zaštitu podataka primjenjuje na SharePoint web-mjestu servisa OneDrive ili određenom artiklu.</span><span class="sxs-lookup"><span data-stu-id="89674-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="89674-104">To uključuje Nemogućnost brisanja dokumenta, verzije dokumenta, mape, biblioteke dokumenata, popisa, aplikacije, web-mjesta ili zbirke web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="89674-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="89674-105">Evo nekih primjera poruka o pogrešci koje možete primiti ako pokušate izbrisati stavku koja se zadržava:</span><span class="sxs-lookup"><span data-stu-id="89674-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="89674-106">"Ovo web-mjesto ne može biti izbrisano jer je uključeno u zadržavanje ili pravila zadržavanja u vezi s pridržavanjem dokumenata"</span><span class="sxs-lookup"><span data-stu-id="89674-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="89674-107">"Ova stranica ima pravila usklađenosti postavljena za blokiranje brisanja"</span><span class="sxs-lookup"><span data-stu-id="89674-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="89674-108">"Politika usklađenosti trenutno blokira brisanje web-mjesta"</span><span class="sxs-lookup"><span data-stu-id="89674-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="89674-109">"Ova zbirka web-mjesta ne može se izbrisati jer sadrži web-mjesta koja su uključena u zadržavanje ili pravila zadržavanja u okviru eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="89674-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="89674-110">"Morate izbrisati sve stavke u ovoj mapi prije nego što izbrišete mapu"</span><span class="sxs-lookup"><span data-stu-id="89674-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="89674-111">"Verzije ove stavke ne mogu se izbrisati jer je na čekanju ili pravila zadržavanja"</span><span class="sxs-lookup"><span data-stu-id="89674-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="89674-112">"Stavka se ne može izbrisati dok je na čekanju"</span><span class="sxs-lookup"><span data-stu-id="89674-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="89674-113">"Oznaka koja se primjenjuje na ovu stavku sprječava njegovo uređivanje ili brisanje"</span><span class="sxs-lookup"><span data-stu-id="89674-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="89674-114">"Popis se ne može izbrisati dok je na čekanju ili pravila zadržavanja"</span><span class="sxs-lookup"><span data-stu-id="89674-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="89674-115">"Popis nije moguće izbrisati ako je blokiran ili se na njega primjenjuje pravila zadržavanja"</span><span class="sxs-lookup"><span data-stu-id="89674-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="89674-116">Da biste izbrisali stavke u jednom od tih scenarija, potrebno je ukloniti pravila zadržavanja, oznaku zadržavanja ili zadržavanje podataka o pravilniku o privatnosti (ili web-mjesto mora biti isključeno iz pravila zadržavanja).</span><span class="sxs-lookup"><span data-stu-id="89674-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="89674-117">Morate onemogućiti ili isključiti odgovarajuće čekanje koje uzrokuje taj problem.</span><span class="sxs-lookup"><span data-stu-id="89674-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="89674-118">Nakon što se pravila zadržavanja ili zadržavanje uklone, može trajati do 24 sata kako bi promjena stupila na snagu.</span><span class="sxs-lookup"><span data-stu-id="89674-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="89674-119">Informacije o različitim značajkama zadržavanja i držanja koja se mogu primijeniti na SharePoint web-mjesta i račune servisa OneDrive potražite u jednoj od sljedećih tema.</span><span class="sxs-lookup"><span data-stu-id="89674-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="89674-120">Pregled pravila zadržavanja</span><span class="sxs-lookup"><span data-stu-id="89674-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="89674-121">Pregled naljepnica zadržavanja</span><span class="sxs-lookup"><span data-stu-id="89674-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="89674-122">Upravljanje čekanjima u programu Advanced eDiscovery</span><span class="sxs-lookup"><span data-stu-id="89674-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="89674-123">eDiscovery drži</span><span class="sxs-lookup"><span data-stu-id="89674-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="89674-124">Pravila zatvaranja i brisanja naslijeđenih web-mjesta</span><span class="sxs-lookup"><span data-stu-id="89674-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
