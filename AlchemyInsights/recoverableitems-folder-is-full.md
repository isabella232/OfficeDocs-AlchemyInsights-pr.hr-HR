---
title: mapa funkcija RecoverableItems 1336 je puna
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741259"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="e1641-102">Mapa s stavkama koje je moguće vratiti je puna</span><span class="sxs-lookup"><span data-stu-id="e1641-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="e1641-103">Za poštanske sandučiće sustava Exchange Online zadano ograničenje prostora za pohranu za mapu s stavkama koje se mogu oporaviti iznosi 30 GB.</span><span class="sxs-lookup"><span data-stu-id="e1641-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="e1641-104">Ograničenje prostora za pohranu za mapu stavke koje se mogu vratiti automatski se povećava na 100 GB ako se poštanski sandučić smješta na zadržavanje sudskog postupka, traženje otkrivanja ili je dodijeljeno pravilima zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="e1641-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="e1641-105">Kada mapa Oporavljene stavke dosegne ograničenje prostora za pohranu, funkcionalnost poštanskog sandučića utječe na sljedeće načine:</span><span class="sxs-lookup"><span data-stu-id="e1641-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="e1641-106">Korisnik ne može izbrisati stavke iz poštanskog sandučića.</span><span class="sxs-lookup"><span data-stu-id="e1641-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="e1641-107">Pomoćnik za upravljane mape ne može izbrisati stavke na temelju postavke oznake zadržavanja ili upravljane mape.</span><span class="sxs-lookup"><span data-stu-id="e1641-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="e1641-108">Za poštanske sandučiće koji imaju omogućen jedan oporavak stavke ili su stavljeni na čekanje, postupak zaštite stranice za kopiranje na pisanje ne može održavati verzije stavki koje je korisnik uredio.</span><span class="sxs-lookup"><span data-stu-id="e1641-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="e1641-109">Za poštanske sandučiće koje imaju omogućeno zapisivanje nadzornog sandučića, ne mogu se spremiti stavke zapisnika nadzora poštanskih sandučića u podmapi revizija u mapi stavke koje se mogu oporaviti.</span><span class="sxs-lookup"><span data-stu-id="e1641-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="e1641-110">Za poštanske sandučiće koji nisu na čekanju administratori mogu koristiti `Search-Mailbox -SearchDumpsterOnly -DeleteContent` naredbu u komponenti Exchange Online PowerShell za brisanje stavki u mapi stavke koje se mogu oporaviti.</span><span class="sxs-lookup"><span data-stu-id="e1641-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="e1641-111">Dodatne informacije potražite u sljedećim temama:</span><span class="sxs-lookup"><span data-stu-id="e1641-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="e1641-112">Traženje i brisanje poruka</span><span class="sxs-lookup"><span data-stu-id="e1641-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="e1641-113">Pretraživanje – poštanski sandučić</span><span class="sxs-lookup"><span data-stu-id="e1641-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="e1641-114">Za poštanske sandučiće koji se nalaze na čekanju administratori moraju ukloniti čekanje da bi izbrisali stavke iz mape s stavkama koje se mogu oporaviti.</span><span class="sxs-lookup"><span data-stu-id="e1641-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="e1641-115">Dodatne informacije potražite u članku [Brisanje stavki u mapi stavke koje se mogu oporaviti u cloud-bazirane poštanske sandučiće na čekanju](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="e1641-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="e1641-116">Da biste spriječili potpunu mapu s stavkama koje se mogu oporaviti, administratori mogu povećati ograničenje prostora za pohranu u mapi stavke koje se mogu vratiti za poštanske sandučiće na čekanju i postaviti pravilnik o zadržavanju poštanskog sandučića koji premješta stavke iz mape stavke koje se mogu vratiti u korisnikov arhivski poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="e1641-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="e1641-117">Pročitajte članak [povećanje kvote stavki koje se mogu oporaviti za poštanske sandučiće na čekanju](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="e1641-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
