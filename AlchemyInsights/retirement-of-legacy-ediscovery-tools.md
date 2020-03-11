---
title: Umirovljenje naslijeđenih alata za predočavanje elektroničkih dokumenata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157532"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="70a84-102">Umirovljenje naslijeđenih alata za predočavanje elektroničkih dokumenata</span><span class="sxs-lookup"><span data-stu-id="70a84-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="70a84-103">Kao rezultat nove i poboljšane funkcionalnosti predočavanja elektroničkih dokumenata u centru za usklađenost sustava Microsoft 365, sljedeći naslijeđeni alati i naredbe za predočavanje elektroničkih dokumenata bit će umirovljeni u narednim mjesecima:</span><span class="sxs-lookup"><span data-stu-id="70a84-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="70a84-104">[Lokalno predočavanje elektroničkih dokumenata](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i Lokalno držanje u centru za [administratore](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="70a84-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="70a84-105">Cmdleti komponente Exchange Online PowerShell koji podržavaju lokalno predočavanje elektroničkih dokumenata i držanja na mjestu.</span><span class="sxs-lookup"><span data-stu-id="70a84-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="70a84-106">(Ovi cmdleti su kolektivno identificirani kao \*-MailboxSearch cmdlets.) To uključuje sljedeće cmdlete:</span><span class="sxs-lookup"><span data-stu-id="70a84-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="70a84-107">Novi poštanski sandučić</span><span class="sxs-lookup"><span data-stu-id="70a84-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="70a84-108">Pretraživanje početnog poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="70a84-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="70a84-109">Pretraživanje poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="70a84-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="70a84-110">Postavljanje pretraživanja poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="70a84-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="70a84-111">Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) u komponenti Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="70a84-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="70a84-112">Sljedeće operacije u API-ju za Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="70a84-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="70a84-113">GetSearchablePoštanski sandučići</span><span class="sxs-lookup"><span data-stu-id="70a84-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="70a84-114">SetHoldOnPoštanski sandučići</span><span class="sxs-lookup"><span data-stu-id="70a84-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="70a84-115">GetHoldOnPoštanski sandučići</span><span class="sxs-lookup"><span data-stu-id="70a84-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="70a84-116">Napredno predočavanje elektroničkog dokumenata za Office 365 v1.0</span><span class="sxs-lookup"><span data-stu-id="70a84-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="70a84-117">**Vremenski slijed za umirovljenje:**</span><span class="sxs-lookup"><span data-stu-id="70a84-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="70a84-118">1. travanj 2020.: nećete moći stvoriti nova pretraživanja i čekanja, ali i dalje možete pokrenuti, uređivati i brisati postojeća pretraživanja na vlastitu odgovornost.</span><span class="sxs-lookup"><span data-stu-id="70a84-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="70a84-119">Microsoftova podrška više neće podržavati lokalno predočavanje & drži u EAC-u.</span><span class="sxs-lookup"><span data-stu-id="70a84-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="70a84-120">Srpanj 1, 2020: In-Place eDiscovery & Drži funkcionalnost u EAC će biti smještenu u načinu rada samo za čitanje.</span><span class="sxs-lookup"><span data-stu-id="70a84-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="70a84-121">To znači da ćete moći ukloniti samo postojeća pretraživanja i držanja.</span><span class="sxs-lookup"><span data-stu-id="70a84-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="70a84-122">**Dodatne informacije potražite u odjeljku**:</span><span class="sxs-lookup"><span data-stu-id="70a84-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="70a84-123">Migracija naslijeđenih pretraživanja predočavanje elektroničkih dokumenata</span><span class="sxs-lookup"><span data-stu-id="70a84-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="70a84-124">Umirovljenje naslijeđenih alata za predočavanje elektroničkih dokumenata</span><span class="sxs-lookup"><span data-stu-id="70a84-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="70a84-125">Najčešća pitanja o unaprijed i na mjestu čekanja</span><span class="sxs-lookup"><span data-stu-id="70a84-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)


