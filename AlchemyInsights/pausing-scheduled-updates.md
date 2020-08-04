---
title: Pauziranje zakazanih ažuriranja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/30/2020
ms.locfileid: "46554913"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="42cf9-102">Pauziranje zakazanih ažuriranja</span><span class="sxs-lookup"><span data-stu-id="42cf9-102">Pausing scheduled updates</span></span>

<span data-ttu-id="42cf9-103">Kada se izda naredba za pauzu, uređaji ne obrađuju naredbu do sljedeće prijave u Intune.</span><span class="sxs-lookup"><span data-stu-id="42cf9-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="42cf9-104">Zbog toga vaši uređaji mogu imati:</span><span class="sxs-lookup"><span data-stu-id="42cf9-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="42cf9-105">Instalirana zakazana ažuriranja prije prijave.</span><span class="sxs-lookup"><span data-stu-id="42cf9-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="42cf9-106">Bio isključen kada ste izdali naredbu za pauzu.</span><span class="sxs-lookup"><span data-stu-id="42cf9-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="42cf9-107">U tom slučaju, kada su uređaji bili ukljuèeni, možda su preuzeli i instalirali zakazana ažuriranja prije prijave.</span><span class="sxs-lookup"><span data-stu-id="42cf9-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>