---
title: 1336 RecoverableItems mapa je puna
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: cfcc69c1b3a59c73037d9a493af4ece86b7b7208
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762072"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="a08ed-102">Mapu oporaviti stavke je pun</span><span class="sxs-lookup"><span data-stu-id="a08ed-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="a08ed-103">Za Exchange Online poštanskim sandučićima u sustavu Office 365, zadano ograničenje prostora za pohranu u mapu oporaviti stavke je 30 GB.</span><span class="sxs-lookup"><span data-stu-id="a08ed-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="a08ed-104">Ograničenje spremišta za mapu oporaviti stavke automatski povećan je na 100 GB ako poštanski sandučić smjestiti na čekanju sudskih procesa, čekanje predočavanja elektroničkih dokumenata ili je dodijeljen pravilo zadržavanja za Office 365.</span><span class="sxs-lookup"><span data-stu-id="a08ed-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="a08ed-105">Kada mapu oporaviti stavke dosegne ograničenje prostora za pohranu, funkcionalnost poštanski sandučić je utjecati na sljedeće načine:</span><span class="sxs-lookup"><span data-stu-id="a08ed-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="a08ed-106">Korisnik ne može izbrisati stavke iz poštanskog sandučića.</span><span class="sxs-lookup"><span data-stu-id="a08ed-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="a08ed-107">Upravljani pomoćnika za mape nije moguće izbrisati stavaka na temelju postavke upravljanih mapa ili oznaka zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="a08ed-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="a08ed-108">Za poštanske sandučiće koji imaju omogućen oporavak jednu stavku ili stavljena na čekanje, zaštita proces kopiju na pisanje stranice nije moguće održavati verzije stavki uredio korisnika.</span><span class="sxs-lookup"><span data-stu-id="a08ed-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="a08ed-109">Za poštanske sandučiće koji imaju poštanski sandučić nadzora omogućeno zapisivanje, stavke evidencije nadzora nema poštanski sandučić možete spremiti u revizije podmapu u mapi oporaviti stavke.</span><span class="sxs-lookup"><span data-stu-id="a08ed-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="a08ed-110">Za poštanske sandučiće koji nisu na čekanju, možete koristiti administratori na `Search-Mailbox -SearchDumpsterOnly -DeleteContent` naredbu u Exchange Online PowerShell izbrisati stavke u mapi oporaviti stavke.</span><span class="sxs-lookup"><span data-stu-id="a08ed-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="a08ed-111">Dodatne informacije potražite u sljedećim temama:</span><span class="sxs-lookup"><span data-stu-id="a08ed-111">For more information, see the following topics:</span></span> 

- [<span data-ttu-id="a08ed-112">Traženje i brisanje poruka</span><span class="sxs-lookup"><span data-stu-id="a08ed-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="a08ed-113">Pretraživanje poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="a08ed-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="a08ed-114">Za poštanske sandučiće koji su na čekanju, administratori imaju uklanjanje čekanja prije možete izbrisane stavke iz mape oporaviti stavke.</span><span class="sxs-lookup"><span data-stu-id="a08ed-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="a08ed-115">Dodatne informacije potražite u [izbrisati stavke u oporaviti stavke mape poštanske sandučiće oblak temelji na čekanju](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a08ed-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="a08ed-116">Da biste spriječili mapu oporaviti stavke postaje pune, administratori možete povećati ograničenje prostora za pohranu oporaviti stavke mapu za poštanske sandučiće na čekanju i postavili pravila zadržavanja poštanski sandučić koje premješta stavke iz mape oporaviti stavke arhiva korisnika poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="a08ed-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="a08ed-117">Pogledajte [povećati oporaviti stavke kvote za poštanske sandučiće na čekanju](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a08ed-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
