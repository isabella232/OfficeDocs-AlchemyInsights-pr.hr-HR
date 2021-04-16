---
title: Umirovljenje naslijeđenih alata za predočavanje elektroničkih elektroničkih podataka
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798541"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="8347b-102">Umirovljenje naslijeđenih alata za predočavanje elektroničkih elektroničkih podataka</span><span class="sxs-lookup"><span data-stu-id="8347b-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="8347b-103">Zbog nove i poboljšane funkcije predočavanja elektroničkih elektroničkih obveza u centru za usklađenost sustava Microsoft 365 sljedeći naslijeđeni alati i naredbe za predočavanje elektroničkih obveza bit će povučeni u sljedećim mjesecima:</span><span class="sxs-lookup"><span data-stu-id="8347b-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="8347b-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [and In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span><span class="sxs-lookup"><span data-stu-id="8347b-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="8347b-105">Cmdleti komponente PowerShell sustava Exchange Online koji podržavaju In-Place predočavanje elektroničkih elektroničkih podataka i In-Place čuvanja.</span><span class="sxs-lookup"><span data-stu-id="8347b-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="8347b-106">(Ti se cmdleti zajednički identificiraju kao cmdleti za \*-MailboxSearch.) To obuhvaća sljedeće cmdlete:</span><span class="sxs-lookup"><span data-stu-id="8347b-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="8347b-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="8347b-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="8347b-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="8347b-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="8347b-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="8347b-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="8347b-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="8347b-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="8347b-111">[Cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) u ljuski PowerShell sustava Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="8347b-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="8347b-112">Sljedeće operacije u API-ju za Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="8347b-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="8347b-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="8347b-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="8347b-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="8347b-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="8347b-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="8347b-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="8347b-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="8347b-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="8347b-117">**Vremenska crta za umirovljenje:**</span><span class="sxs-lookup"><span data-stu-id="8347b-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="8347b-118">**1. srpnja 2020.** Više ne možete stvarati nova pretraživanja i zadržavanja, ali postojeće pretraživanja možete pokrenuti, uređivati i brisati na vlastitu odgovornost.</span><span class="sxs-lookup"><span data-stu-id="8347b-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="8347b-119">Microsoftova podrška više ne podržava In-Place eDiscovery & čuvanja u EAC-u.</span><span class="sxs-lookup"><span data-stu-id="8347b-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="8347b-120">**1. listopada 2020** In-Place eDiscovery & Holds funkcionalnost u EAC-u bit će smještena u načinu samo za čitanje, pa možete ukloniti samo postojeća pretraživanja i čuvanja.</span><span class="sxs-lookup"><span data-stu-id="8347b-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="8347b-121">**Dodatne informacije potražite u članku**:</span><span class="sxs-lookup"><span data-stu-id="8347b-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="8347b-122">Migracija naslijeđenih pretraživanja i čuvanja predočavanja elektroničkih elektroničkih obveza u centar za usklađenost sustava Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8347b-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="8347b-123">Umirovljenje naslijeđenih alata za predočavanje elektroničkih elektroničkih podataka</span><span class="sxs-lookup"><span data-stu-id="8347b-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="8347b-124">Najčešća pitanja o In-Place predočavanja elektroničkih In-Place čuvanja</span><span class="sxs-lookup"><span data-stu-id="8347b-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



