---
title: Problemi s performansama za Microsoft Defender za krajnju točku u sustavu Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793637"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="63599-102">Problemi s performansama za Microsoft Defender za krajnju točku u sustavu Linux</span><span class="sxs-lookup"><span data-stu-id="63599-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="63599-103">Ovaj vas članak vodi kroz korake utvrđivanja problema s performansama za Microsoft Defender za krajnju točku u sustavu Linux.</span><span class="sxs-lookup"><span data-stu-id="63599-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="63599-104">Važno je najprije provjeriti je li problem na koji nailazite riješen najnovijom [verzijom](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="63599-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="63599-105">Da biste pokrenuli istragu, pogledajte [članak Otklanjanje poteškoća s performansama za Microsoft Defender za krajnju točku u sustavu Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span><span class="sxs-lookup"><span data-stu-id="63599-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="63599-106">Izuzimanja</span><span class="sxs-lookup"><span data-stu-id="63599-106">Exclusions</span></span>

<span data-ttu-id="63599-107">Izuzimanja mogu pomoći u ublažavanju problema s performansama.</span><span class="sxs-lookup"><span data-stu-id="63599-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="63599-108">Prije početka pregledajte izuzimanja da bi se znalo i dokumentovalo sve dodatne rizike.</span><span class="sxs-lookup"><span data-stu-id="63599-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="63599-109">Dodatne informacije potražite u članku Konfiguriranje [i provjera valjanosti izuzimanja za Microsoft Defender za krajnju točku u sustavu Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="63599-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="63599-110">Kada imate više datoteka & koje želite izuzeti, a sve su one na istoj mountpoint, lakše je isključiti mountpoint.</span><span class="sxs-lookup"><span data-stu-id="63599-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="63599-111">Počevši od izdanja 101.22.80 iz veljače, možete izuzeti cijelu mountpoint.</span><span class="sxs-lookup"><span data-stu-id="63599-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="63599-112">Na primjer, ako je /mnt/backup mountpoint, možete dodati /mnt/backup na popis izuzetih pokretanjem ove naredbe:</span><span class="sxs-lookup"><span data-stu-id="63599-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="63599-113">**Napomena:** dodavanjem izuzimanja povećava se rizik da se zlonamjerni softver ne otkrije te se njima treba oprezno rukovati i implementirati.</span><span class="sxs-lookup"><span data-stu-id="63599-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="63599-114">Potrebna vam je pomoć?</span><span class="sxs-lookup"><span data-stu-id="63599-114">Need Help?</span></span>

<span data-ttu-id="63599-115">Da biste vam pomogli na najučinkovitiji način, prikupite dijagnostičke podatke prije otvaranja slučaja podrške.</span><span class="sxs-lookup"><span data-stu-id="63599-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
