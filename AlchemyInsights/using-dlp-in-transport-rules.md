---
title: Upotreba DLP-a u pravilima prijenosa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915048"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="6294e-102">Upotreba DLP-a u pravilima prijenosa</span><span class="sxs-lookup"><span data-stu-id="6294e-102">Using DLP in transport rules</span></span>

<span data-ttu-id="6294e-103">Da biste u postojeći transport integrirali sprječavanje gubitka podataka (DLP), upotrijebite uvjet „**Ako poruka sadrži...Osjetljive informacije**” u postavci pravila prijenosa.</span><span class="sxs-lookup"><span data-stu-id="6294e-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="6294e-104">**Dodatne detalje potražite u sljedećem članku:**</span><span class="sxs-lookup"><span data-stu-id="6294e-104">**For more details, see:**</span></span>

- <span data-ttu-id="6294e-105">Integrirane vrste osjetljivih informacija za DLP u pravilima prijenosa: [integriranje pravila o osjetljivim informacijama](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="6294e-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="6294e-106">Pravilo ujedno možete testirati sa ili bez testa pravilnika s pomoću načina za testiranje na pravilu.</span><span class="sxs-lookup"><span data-stu-id="6294e-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="6294e-107">Prije testiranja biste trebali pričekati 30 minuta nakon stvaranja pravila.</span><span class="sxs-lookup"><span data-stu-id="6294e-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="6294e-108">Pogledajte [Testiranje pravila tijeka/prijenosa pošte](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="6294e-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="6294e-109">**Napomena**: ako pokušavate implementirati novi DLP pravilnik s pravilnikom prijenosa u EAC-u, umjesto toga upotrijebite pravilnike [DLP-a u centru za sigurnost i usklađivanje](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="6294e-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
