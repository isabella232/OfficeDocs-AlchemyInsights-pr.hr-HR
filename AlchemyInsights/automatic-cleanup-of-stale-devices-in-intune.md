---
title: Automatsko čišćenje ustajalih uređaja u intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554772"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="cc6d9-102">Automatsko čišćenje ustajalih uređaja u intune</span><span class="sxs-lookup"><span data-stu-id="cc6d9-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="cc6d9-103">Intune omogućuje admin konfigurirati vremenski interval između 90 i 270 dana, nakon čega ustajali uređaji su uklonjeni iz usluge.</span><span class="sxs-lookup"><span data-stu-id="cc6d9-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="cc6d9-104">Ova postavka je organizacija široka i nakon što se aktivira stupa na snagu odmah.</span><span class="sxs-lookup"><span data-stu-id="cc6d9-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="cc6d9-105">Svi uređaji koji nisu prijavljeni na Intune poslužitelj u razdoblju koje premašuje postavku trajno se brišu.</span><span class="sxs-lookup"><span data-stu-id="cc6d9-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="cc6d9-106">**Napomena:** Samo objekti MDM uređaja ispunjavaju uvjete za ovu akciju čišćenja.</span><span class="sxs-lookup"><span data-stu-id="cc6d9-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="cc6d9-107">Isključeni su samo objekti uređaja EAS- a.</span><span class="sxs-lookup"><span data-stu-id="cc6d9-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="cc6d9-108">Za dodatne informacije o tome kada uređaj ispunjava uvjete za brisanje na temelju postavke čišćenja uređaja i njezina "stanja":</span><span class="sxs-lookup"><span data-stu-id="cc6d9-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="cc6d9-109">Postavka: **brisanje uređaja nakon zadnjeg datuma prijave: Da (neka vrijednost (N) u navedenim danima)**</span><span class="sxs-lookup"><span data-stu-id="cc6d9-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="cc6d9-110">Na temelju vrijednosti (N) konfigurirane u postavci, servis Intune briše uređaj u navedenim danima nakon zadnje uspješne prijave.</span><span class="sxs-lookup"><span data-stu-id="cc6d9-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="cc6d9-111">Postavka: **brisanje uređaja nakon zadnjeg datuma prijave: Ne**</span><span class="sxs-lookup"><span data-stu-id="cc6d9-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="cc6d9-112">180 dana nakon isteka certifikata uređaja i ne obnavlja se, uređaj se briše.</span><span class="sxs-lookup"><span data-stu-id="cc6d9-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="cc6d9-113">**Napomena:** U oba slučaja uređaj mora biti uspješno registriran u Intuneu.</span><span class="sxs-lookup"><span data-stu-id="cc6d9-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="cc6d9-114">Registracija se događa tijekom prve provjere uređaja s uslugom Intune.</span><span class="sxs-lookup"><span data-stu-id="cc6d9-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="cc6d9-115">Ako se uređaj uspješno upiše u Intune, ali ne postane registriran u Intuneu, uređaj se briše 270 dana nakon prijave.</span><span class="sxs-lookup"><span data-stu-id="cc6d9-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="cc6d9-116">(90 dana za označavanje uređaja kao opozvanog, a zatim još 180 dana za brisanje zapisa.)</span><span class="sxs-lookup"><span data-stu-id="cc6d9-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="cc6d9-117">Trenutno ne postoji mehanizam u intune konzoli kako bi se utvrdio datum isteka certifikata uređaja za bilo koji uređaj.</span><span class="sxs-lookup"><span data-stu-id="cc6d9-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>