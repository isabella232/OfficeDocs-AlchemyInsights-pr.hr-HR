---
title: Status senzora provjere krajnje točke programa Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676056"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="ec379-102">Status senzora provjere krajnje točke programa Defender</span><span class="sxs-lookup"><span data-stu-id="ec379-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="ec379-103">Pločica **Uređaji s problemima sa senzorom** nalazi se na nadzornoj ploči sigurnosnih operacija.</span><span class="sxs-lookup"><span data-stu-id="ec379-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="ec379-104">Ova pločica sadrži informacije o mogućnosti pojedinačnog uređaja za pružanje podataka senzora i komunikaciju sa servisom Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="ec379-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="ec379-105">U njemu se izvješćuje koliko je uređaja potrebno obratiti pozornost i pomaže vam prepoznati problematične uređaje i poduzeti radnje za ispravljanje poznatih problema.</span><span class="sxs-lookup"><span data-stu-id="ec379-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="ec379-106">Dva pokazatelja statusa na pločici pružaju informacije o broju uređaja koji se ne prijave pravilno servisu:</span><span class="sxs-lookup"><span data-stu-id="ec379-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="ec379-107">**Pogrešno konfigurirano** Uređaji koji djelomično izvješćuju o podacima senzora servisu Defender for Endpoint i mogu imati konfiguracijske pogreške koje je potrebno ispraviti.</span><span class="sxs-lookup"><span data-stu-id="ec379-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="ec379-108">**Neaktivno** Uređaji koji su u proteklom mjesecu prestali izvješćivanju o servisu Defender za krajnju točku više od sedam dana.</span><span class="sxs-lookup"><span data-stu-id="ec379-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="ec379-109">Klikom na neku od grupa usmjeravate se na popis Uređaji filtrirani prema vašim izborima.</span><span class="sxs-lookup"><span data-stu-id="ec379-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="ec379-110">Na popisu Uređaji popis stanja stanja možete filtrirati prema sljedećem statusu:</span><span class="sxs-lookup"><span data-stu-id="ec379-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="ec379-111">**Aktivno** Uređaji koji aktivno izvješćuju servisu Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="ec379-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="ec379-112">**Pogrešno konfigurirano** Uređaji koji djelomično izvješćuju o podacima senzora servisu Defender for Endpoint, ali imaju konfiguracijske pogreške koje je potrebno ispraviti.</span><span class="sxs-lookup"><span data-stu-id="ec379-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="ec379-113">Pogrešno konfigurirani uređaji mogu imati jedan ili kombinaciju sljedećih problema:</span><span class="sxs-lookup"><span data-stu-id="ec379-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="ec379-114">Nema podataka o senzoru – uređaji su prestali slati podatke senzora.</span><span class="sxs-lookup"><span data-stu-id="ec379-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="ec379-115">S uređaja se mogu pokrenuti ograničena upozorenja.</span><span class="sxs-lookup"><span data-stu-id="ec379-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="ec379-116">Oštećena komunikacija – smanjena je mogućnost komunikacije s uređajem.</span><span class="sxs-lookup"><span data-stu-id="ec379-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="ec379-117">Slanje datoteka radi dubinske analize, blokiranje datoteka, izolacija uređaja od mreže i drugih akcija koje zahtijevaju komunikaciju s uređajem možda neće funkcionirati.</span><span class="sxs-lookup"><span data-stu-id="ec379-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="ec379-118">**Neaktivno** Uređaji koji su prestali s izvješćivanjem o servisu Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="ec379-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="ec379-119">Cijeli popis možete preuzeti u CSV obliku pomoću značajke Izvoz.</span><span class="sxs-lookup"><span data-stu-id="ec379-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="ec379-120">Dodatne informacije potražite u članku Provjera [stanja senzora u programu Microsoft Defender za krajnju točku](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="ec379-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="ec379-121">Dodatne informacije o tome što je uzrokovalo neaktivnost ili pogrešno konfiguriranje uređaja potražite u članku Rješavanje nezdravih [senzora u programu Microsoft Defender za krajnju točku](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="ec379-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
