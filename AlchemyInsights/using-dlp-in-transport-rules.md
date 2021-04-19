---
title: Upotreba DLP-a u pravilima prijenosa
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
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827208"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="00abd-102">Upotreba DLP-a u pravilima prijenosa</span><span class="sxs-lookup"><span data-stu-id="00abd-102">Using DLP in transport rules</span></span>

<span data-ttu-id="00abd-103">Da biste u postojeći transport integrirali sprječavanje gubitka podataka (DLP), upotrijebite uvjet „**Ako poruka sadrži...Osjetljive informacije**” u postavci pravila prijenosa.</span><span class="sxs-lookup"><span data-stu-id="00abd-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="00abd-104">**Dodatne detalje potražite u sljedećem članku:**</span><span class="sxs-lookup"><span data-stu-id="00abd-104">**For more details, see:**</span></span>

- <span data-ttu-id="00abd-105">Integrirane vrste osjetljivih informacija za DLP u pravilima prijenosa: [integriranje pravila o osjetljivim informacijama](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="00abd-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="00abd-106">Pravilo ujedno možete testirati sa ili bez testa pravilnika s pomoću načina za testiranje na pravilu.</span><span class="sxs-lookup"><span data-stu-id="00abd-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="00abd-107">Prije testiranja biste trebali pričekati 30 minuta nakon stvaranja pravila.</span><span class="sxs-lookup"><span data-stu-id="00abd-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="00abd-108">Pogledajte [Testiranje pravila tijeka/prijenosa pošte](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="00abd-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="00abd-109">**Napomena**: ako pokušavate implementirati novi DLP pravilnik s pravilnikom prijenosa u EAC-u, umjesto toga upotrijebite pravilnike [DLP-a u centru za sigurnost i usklađivanje](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="00abd-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
