---
title: Otklanjanje poteškoća s događajima iz poruke e-pošte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834831"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="27bb4-102">Otklanjanje poteškoća s događajima iz poruke e-pošte</span><span class="sxs-lookup"><span data-stu-id="27bb4-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="27bb4-103">Provjera je li značajka omogućena za poštanski sandučić: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="27bb4-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="27bb4-104">Zatim pogledajte zapisnike "Događaji iz **e-pošte" Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="27bb4-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="27bb4-105">U zapisnicima "Događaji iz e-pošte" pronađite InternetMessageId koji odgovara stavci u poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="27bb4-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="27bb4-106">TrustScore određuje je li stavka dodana ili nije.</span><span class="sxs-lookup"><span data-stu-id="27bb4-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="27bb4-107">Događaji će se dodati samo ako je TrustScore = "Pouzdano".</span><span class="sxs-lookup"><span data-stu-id="27bb4-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="27bb4-108">TrustScore određuje SPF, Dkim ili Dmarc svojstva koja se nalaze u zaglavlju poruke.</span><span class="sxs-lookup"><span data-stu-id="27bb4-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="27bb4-109">Da biste pogledali ova svojstva:</span><span class="sxs-lookup"><span data-stu-id="27bb4-109">To view these properties:</span></span>

<span data-ttu-id="27bb4-110">**Outlook za stolna računala**</span><span class="sxs-lookup"><span data-stu-id="27bb4-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="27bb4-111">Otvaranje stavke</span><span class="sxs-lookup"><span data-stu-id="27bb4-111">Open the item</span></span>
- <span data-ttu-id="27bb4-112">Svojstva datoteka -> -> Internet Headers</span><span class="sxs-lookup"><span data-stu-id="27bb4-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="27bb4-113">ili</span><span class="sxs-lookup"><span data-stu-id="27bb4-113">or</span></span>

<span data-ttu-id="27bb4-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="27bb4-114">**MFCMapi**</span></span>

- <span data-ttu-id="27bb4-115">Prelazak na stavku u ulaznoj pošti</span><span class="sxs-lookup"><span data-stu-id="27bb4-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="27bb4-116">Potražite PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="27bb4-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="27bb4-117">Ta se svojstva određuju i bilježe tijekom prijenosa i usmjeravanja.</span><span class="sxs-lookup"><span data-stu-id="27bb4-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="27bb4-118">Da biste dodatno otkloniti poteškoće, možda ćete morati nastaviti s podrškom za transport o pogreškama u SPF-u, DKIM-u i.ili DMARC-u.</span><span class="sxs-lookup"><span data-stu-id="27bb4-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>