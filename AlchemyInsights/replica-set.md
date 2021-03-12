---
title: Skup replika
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713497"
---
# <a name="replica-set"></a><span data-ttu-id="09380-102">Skup replika</span><span class="sxs-lookup"><span data-stu-id="09380-102">Replica set</span></span>

<span data-ttu-id="09380-103">Dodatak se naziva i kao upravljana domena.</span><span class="sxs-lookup"><span data-stu-id="09380-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="09380-104">To je zapravo dva kontrolora domene koji se pokreću i održavaju u pozadini.</span><span class="sxs-lookup"><span data-stu-id="09380-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="09380-105">Dva DCs uključuju jedan glavni DC i jedan Replikacijski DC.</span><span class="sxs-lookup"><span data-stu-id="09380-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="09380-106">Sigurnosne kopije u ZBRAJANJEM (upravljana domena) automatizirani su postupak koji upravlja platformom Azure.</span><span class="sxs-lookup"><span data-stu-id="09380-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="09380-107">U slučaju problema s upravljanom domenom, Podrška za Azure može vam pomoći u vraćanju iz sigurnosne kopije.</span><span class="sxs-lookup"><span data-stu-id="09380-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="09380-108">Svaki skup replika stvarate u virtualnoj mreži.</span><span class="sxs-lookup"><span data-stu-id="09380-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="09380-109">Svaka Virtualna mreža mora biti postavljena na svaku drugu virtualnu mrežu koja sadrži skup replika upravljanih domena.</span><span class="sxs-lookup"><span data-stu-id="09380-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="09380-110">Ta konfiguracija stvara topologiju Mesh Network koja podržava replikaciju imenika.</span><span class="sxs-lookup"><span data-stu-id="09380-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="09380-111">Virtualna mreža može podržavati višestruke skupove replika, pod uvjetom da je svaki skup replika u nekoj drugoj virtualnoj subnetu.</span><span class="sxs-lookup"><span data-stu-id="09380-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="09380-112">Dodatne informacije o skupu replika potražite u članku [Koncepti Skupovi replika](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="09380-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
