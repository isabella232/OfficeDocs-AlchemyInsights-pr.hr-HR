---
title: Softverski inventar nedostaje ili je netočan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676143"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="deead-102">Softverski inventar nedostaje ili je netočan</span><span class="sxs-lookup"><span data-stu-id="deead-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="deead-103">Softverski inventar u upravljanje prijetnjama i ranjivostima (TVM) popis je poznatih softvera u vašoj tvrtki ili ustanovi sa službenim Enumeracijama Common Platform (CPE).</span><span class="sxs-lookup"><span data-stu-id="deead-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="deead-104">Softverski proizvodi bez službenog CPE-a ne objavljuju slabe točke.</span><span class="sxs-lookup"><span data-stu-id="deead-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="deead-105">Inventar obuhvaća i pojedinosti kao što su naziv dobavljača, broj nedostataka, prijetnji i broj izloženih uređaja.</span><span class="sxs-lookup"><span data-stu-id="deead-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="deead-106">Promjene softvera na uređajima obično se odražavaju na sigurnosnim portalima u roku od dva sata.</span><span class="sxs-lookup"><span data-stu-id="deead-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="deead-107">No katkad je potrebno i dulje.</span><span class="sxs-lookup"><span data-stu-id="deead-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="deead-108">Trenutno ne postoji način prisile sinkronizacije; to je kontinuirana procjena.</span><span class="sxs-lookup"><span data-stu-id="deead-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="deead-109">Ako ste promijenili softver i promjena se ne odražava točno u TVM-u nakon 5 sati, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="deead-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="deead-110">U odjeljku softverski dokaz provjerite kako je softver otkriven.</span><span class="sxs-lookup"><span data-stu-id="deead-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="deead-111">Provjerite je li softver podržan.</span><span class="sxs-lookup"><span data-stu-id="deead-111">Make sure that the software is supported.</span></span> <span data-ttu-id="deead-112">Softver može biti vidljiv samo na razini uređaja čak i ako ga trenutno ne podržava upravljanje prijetnjama i ranjivostima.</span><span class="sxs-lookup"><span data-stu-id="deead-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="deead-113">No dostupni su samo ograničeni podaci.</span><span class="sxs-lookup"><span data-stu-id="deead-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="deead-114">Upute za prijavu netočnosti s portala pogledajte u članku Prijava [netočnosti](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="deead-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="deead-115">**Napomena:** izvješćivanje o netočnosti s portala MDE jednosmjerni je kanal za inženjering.</span><span class="sxs-lookup"><span data-stu-id="deead-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="deead-116">Ako je problem hitan, otvorite kartu za podršku.</span><span class="sxs-lookup"><span data-stu-id="deead-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="deead-117">Dodatne informacije potražite u članku [Inventar softvera – upravljanje prijetnjama i ranjivostima](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="deead-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>