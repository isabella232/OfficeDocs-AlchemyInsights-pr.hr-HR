---
title: Povlačenje naslijeđenih alata za otkriće
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727775"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="0733f-102">Povlačenje naslijeđenih alata za otkriće</span><span class="sxs-lookup"><span data-stu-id="0733f-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="0733f-103">Kao rezultat nove i poboljšane funkcionalnosti otkrivanja sustava Microsoft 365, u sljedećim mjesecima bit će umirovljen sljedeći Alati za otkrivanje naslijeđenih i naredbina:</span><span class="sxs-lookup"><span data-stu-id="0733f-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="0733f-104">U centru za administratore sustava Exchange [na mjestu e-otkrivanje](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i [mjesto](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)</span><span class="sxs-lookup"><span data-stu-id="0733f-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="0733f-105">Cmdleti za Exchange Online PowerShell koji podržavaju web-otkriće i web-mjesto koje sadrži.</span><span class="sxs-lookup"><span data-stu-id="0733f-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="0733f-106">(Ovi su cmdleti kolektivno identificirani za cmdlete \*-MailboxSearch.) To obuhvaća sljedeće cmdlete:</span><span class="sxs-lookup"><span data-stu-id="0733f-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="0733f-107">Novo-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="0733f-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="0733f-108">Početak – MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="0733f-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="0733f-109">Zaustavljanje-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="0733f-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="0733f-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="0733f-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="0733f-111">Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) u komponenti Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0733f-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="0733f-112">Sljedeće operacije u API-ju sustava Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="0733f-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="0733f-113">Getsearchablepoštanske sandučiće</span><span class="sxs-lookup"><span data-stu-id="0733f-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="0733f-114">Setholdonsandučići</span><span class="sxs-lookup"><span data-stu-id="0733f-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="0733f-115">Getholdonsandučići</span><span class="sxs-lookup"><span data-stu-id="0733f-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="0733f-116">Napredno Idiscovery v 1,0</span><span class="sxs-lookup"><span data-stu-id="0733f-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="0733f-117">**Vremenska traka za mirovinu**:</span><span class="sxs-lookup"><span data-stu-id="0733f-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="0733f-118">**Srpanj 1, 2020** Više ne možete stvarati nova pretraživanja i održavati, no možete pokrenuti, uređivati i brisati postojeća pretraživanja na vlastitu odgovornost.</span><span class="sxs-lookup"><span data-stu-id="0733f-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="0733f-119">Microsoftova podrška više ne podržava e-otkrivanje na mjestu & drži u sustavu e-servisa.</span><span class="sxs-lookup"><span data-stu-id="0733f-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="0733f-120">**1. listopada 2020** U načinu rada za idiscovery & sadrži funkcionalnost u programu IAC bit će postavljena samo za čitanje, pa možete ukloniti samo postojeća pretraživanja i sadrži.</span><span class="sxs-lookup"><span data-stu-id="0733f-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="0733f-121">Dodatne **informacije potražite u članku**:</span><span class="sxs-lookup"><span data-stu-id="0733f-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="0733f-122">Migraciju naslijeđenih pretraživanja u programu Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0733f-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="0733f-123">Povlačenje naslijeđenih alata za otkriće</span><span class="sxs-lookup"><span data-stu-id="0733f-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="0733f-124">Najčešća pitanja o Neotkrivanjem na servisu i servisu na mjestu</span><span class="sxs-lookup"><span data-stu-id="0733f-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



