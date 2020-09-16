---
title: Otklanjanje poteškoća s e-poštom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658726"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="3c14f-102">Otklanjanje poteškoća s e-poštom</span><span class="sxs-lookup"><span data-stu-id="3c14f-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="3c14f-103">Provjera je li značajka omogućena za poštanski sandučić: \*\*dohvaćanje-EventsFromEmailConfiguration – Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="3c14f-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="3c14f-104">Zatim pogledajte "događaji iz poruka e-pošte" **Export-Mailboxdijagnostički zapisnici <mailbox> -komponenta timeprofile**</span><span class="sxs-lookup"><span data-stu-id="3c14f-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="3c14f-105">U zapisnicima "događaji iz e-pošte" Pronađite aplikaciju InternetMessageId koja odgovara stavci u poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="3c14f-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="3c14f-106">Rezultat pouzdanosti određuje je li stavka dodana ili nije.</span><span class="sxs-lookup"><span data-stu-id="3c14f-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="3c14f-107">Događaji će se dodati samo ako je TrustScore = "pouzdan".</span><span class="sxs-lookup"><span data-stu-id="3c14f-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="3c14f-108">Funkcija TrustScore određuje se pomoću funkcija SPF, depet ili DeMarka, koje se nalaze u zaglavlju poruke.</span><span class="sxs-lookup"><span data-stu-id="3c14f-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="3c14f-109">Da biste pogledali ta svojstva, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="3c14f-109">To view these properties:</span></span>

<span data-ttu-id="3c14f-110">**Outlook za stolna računala**</span><span class="sxs-lookup"><span data-stu-id="3c14f-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="3c14f-111">Otvaranje stavke</span><span class="sxs-lookup"><span data-stu-id="3c14f-111">Open the item</span></span>
- <span data-ttu-id="3c14f-112">Svojstva datoteka->-> Internetska zaglavlja</span><span class="sxs-lookup"><span data-stu-id="3c14f-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="3c14f-113">ili</span><span class="sxs-lookup"><span data-stu-id="3c14f-113">or</span></span>

<span data-ttu-id="3c14f-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="3c14f-114">**MFCMapi**</span></span>

- <span data-ttu-id="3c14f-115">Navigacija do stavke u ulaznoj pošti</span><span class="sxs-lookup"><span data-stu-id="3c14f-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="3c14f-116">Potražite PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="3c14f-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="3c14f-117">Ta se svojstva određuju i snimaju tijekom transporta i proizvodnog postupka.</span><span class="sxs-lookup"><span data-stu-id="3c14f-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="3c14f-118">Da biste dodatno otklanjanja poteškoća, možda ćete morati pratiti podršku za transport o neuspjehom u programu SPF, DKIM i. ili DMARC.</span><span class="sxs-lookup"><span data-stu-id="3c14f-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>