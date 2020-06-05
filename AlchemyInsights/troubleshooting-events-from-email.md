---
title: Otklanjanje poteškoća s događajima iz e-pošte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44568941"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="c3455-102">Otklanjanje poteškoća s događajima iz e-pošte</span><span class="sxs-lookup"><span data-stu-id="c3455-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="c3455-103">Provjerite je li značajka omogućena za poštanski sandučić: \*\*Get-EventsFromEmailConfiguration -Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="c3455-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="c3455-104">Zatim pogledajte 'Događaji iz e-pošte' trupaca **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="c3455-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="c3455-105">U zapisnicima "Događaji iz e-pošte" pronađite InternetMessageId koji odgovara stavci u poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="c3455-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="c3455-106">TrustScore određuje je li stavka dodana ili ne.</span><span class="sxs-lookup"><span data-stu-id="c3455-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="c3455-107">Događaji će se dodati samo ako trustscore = "Pouzdano".</span><span class="sxs-lookup"><span data-stu-id="c3455-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="c3455-108">TrustScore je određen SPF, Dkim ili Dmarc svojstvima, koja se nalaze u zaglavlju poruke.</span><span class="sxs-lookup"><span data-stu-id="c3455-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="c3455-109">Da biste pregledali ova svojstva:</span><span class="sxs-lookup"><span data-stu-id="c3455-109">To view these properties:</span></span>

<span data-ttu-id="c3455-110">**Outlook za radnu površinu**</span><span class="sxs-lookup"><span data-stu-id="c3455-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="c3455-111">Otvaranje stavke</span><span class="sxs-lookup"><span data-stu-id="c3455-111">Open the item</span></span>
- <span data-ttu-id="c3455-112">File -> Properties -> Internet Headers</span><span class="sxs-lookup"><span data-stu-id="c3455-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="c3455-113">Ili</span><span class="sxs-lookup"><span data-stu-id="c3455-113">or</span></span>

<span data-ttu-id="c3455-114">**MFCMapi (U**</span><span class="sxs-lookup"><span data-stu-id="c3455-114">**MFCMapi**</span></span>

- <span data-ttu-id="c3455-115">Navigacija do stavke u pristigloj pošti</span><span class="sxs-lookup"><span data-stu-id="c3455-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="c3455-116">Potražite PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="c3455-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="c3455-117">Ta se svojstva određuju i bilježe tijekom prijevoza i usmjeravanja.</span><span class="sxs-lookup"><span data-stu-id="c3455-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="c3455-118">Za daljnje otklanjanje poteškoća, možda ćete morati pratiti uz podršku za promet o kvarovima u SPF, DKIM i.ili DMARC.</span><span class="sxs-lookup"><span data-stu-id="c3455-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>