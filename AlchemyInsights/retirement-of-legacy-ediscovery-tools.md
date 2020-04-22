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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650560"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="c0c85-102">Umirovljenje naslijeđenih alata za predočavanje elektroničkih dokumenata</span><span class="sxs-lookup"><span data-stu-id="c0c85-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="c0c85-103">Kao rezultat nove i poboljšane funkcije predočavanja elektroničkih dokumenata u centru za usklađenost sustava Microsoft 365, sljedeći naslijeđeni alati i naredbe za predočavanje elektroničkih dokumenata bit će umirovljeni u narednim mjesecima:</span><span class="sxs-lookup"><span data-stu-id="c0c85-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="c0c85-104">[Lokalno predočavanje elektroničkih dokumenata](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i lokalno čekanje u centru za [administratore](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0c85-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="c0c85-105">Cmdleti komponente Exchange Online PowerShell koji podržavaju lokalno predočavanje elektroničkih dokumenata i lokalno čekanje.</span><span class="sxs-lookup"><span data-stu-id="c0c85-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="c0c85-106">(Ti su cmdleti zajednički identificirani kao cmdleti \*-MailboxSearch.) To uključuje sljedeće cmdlete:</span><span class="sxs-lookup"><span data-stu-id="c0c85-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="c0c85-107">Novo pretraživanje poštanskih sandučića</span><span class="sxs-lookup"><span data-stu-id="c0c85-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="c0c85-108">Početno pretraživanje poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="c0c85-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="c0c85-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c0c85-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="c0c85-110">Postavljanje pretraživanja poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="c0c85-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="c0c85-111">Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) u komponenti Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c0c85-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="c0c85-112">Sljedeće operacije u API-ju exchange web-usluga:</span><span class="sxs-lookup"><span data-stu-id="c0c85-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="c0c85-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c0c85-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="c0c85-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c0c85-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="c0c85-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c0c85-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="c0c85-116">Napredno predočavanje elektroničkih dokumenata v1.0</span><span class="sxs-lookup"><span data-stu-id="c0c85-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="c0c85-117">**Rokovi za umirovljenje:**</span><span class="sxs-lookup"><span data-stu-id="c0c85-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="c0c85-118">1. travanj 2020: nećete moći stvoriti nova pretraživanja i drži, ali još uvijek možete pokrenuti, urediti i izbrisati postojeća pretraživanja na vlastitu odgovornost.</span><span class="sxs-lookup"><span data-stu-id="c0c85-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="c0c85-119">Microsoftova podrška više neće podržavati lokalno predočavanje elektroničkih dokumenata & u EAC-u.</span><span class="sxs-lookup"><span data-stu-id="c0c85-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="c0c85-120">1. srpanj 2020.: Funkcija otkrivanja elektroničkih dokumenata na mjestu & u EAC-u bit će smještena u načinu rada samo za čitanje.</span><span class="sxs-lookup"><span data-stu-id="c0c85-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="c0c85-121">To znači da ćete moći ukloniti samo postojeća pretraživanja i čekanja.</span><span class="sxs-lookup"><span data-stu-id="c0c85-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="c0c85-122">**Dodatne informacije potražite u odjeljku**:</span><span class="sxs-lookup"><span data-stu-id="c0c85-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="c0c85-123">Migriranje naslijeđenih pretraživanja i čekanja na microsoft 365 centar za usklađenost</span><span class="sxs-lookup"><span data-stu-id="c0c85-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="c0c85-124">Umirovljenje naslijeđenih alata za predočavanje elektroničkih dokumenata</span><span class="sxs-lookup"><span data-stu-id="c0c85-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="c0c85-125">Najčešća pitanja o otkrivanju elektroničkih dokumenata na mjestu i zasima zamjenom</span><span class="sxs-lookup"><span data-stu-id="c0c85-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



