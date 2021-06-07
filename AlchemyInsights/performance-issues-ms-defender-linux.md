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
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Problemi s performansama za Microsoft Defender za krajnju točku u sustavu Linux

Ovaj vas članak vodi kroz korake utvrđivanja problema s performansama za Microsoft Defender za krajnju točku u sustavu Linux.

Važno je najprije provjeriti je li problem na koji nailazite riješen najnovijom [verzijom](/microsoft-365/security/defender-endpoint/linux-whatsnew). 

Da biste pokrenuli istragu, pogledajte [članak Otklanjanje poteškoća s performansama za Microsoft Defender za krajnju točku u sustavu Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).

## <a name="exclusions"></a>Izuzimanja

Izuzimanja mogu pomoći u ublažavanju problema s performansama. Prije početka pregledajte izuzimanja da bi se znalo i dokumentovalo sve dodatne rizike.

Dodatne informacije potražite u članku Konfiguriranje [i provjera valjanosti izuzimanja za Microsoft Defender za krajnju točku u sustavu Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).

Kada imate više datoteka & koje želite izuzeti, a sve su one na istoj mountpoint, lakše je isključiti mountpoint. Počevši od izdanja 101.22.80 iz veljače, možete izuzeti cijelu mountpoint.

Na primjer, ako je /mnt/backup mountpoint, možete dodati /mnt/backup na popis izuzetih pokretanjem ove naredbe:

`$ mdatp exclusion folder add –path /mnt/backup`

**Napomena:** dodavanjem izuzimanja povećava se rizik da se zlonamjerni softver ne otkrije te se njima treba oprezno rukovati i implementirati.

## <a name="need-help"></a>Potrebna vam je pomoć?

Da biste vam pomogli na najučinkovitiji način, prikupite dijagnostičke podatke prije otvaranja slučaja podrške.
