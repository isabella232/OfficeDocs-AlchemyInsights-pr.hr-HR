---
title: Automatsko čišćenje ustajalih uređaja u programu Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715013"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="6c1d8-102">Automatsko čišćenje ustajalih uređaja u programu Intune</span><span class="sxs-lookup"><span data-stu-id="6c1d8-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="6c1d8-103">Intune administratore omogućuje konfiguriranje vremenskog intervala između 90 i 270 dana, nakon čega se ustajali uređaji uklanjaju iz servisa.</span><span class="sxs-lookup"><span data-stu-id="6c1d8-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="6c1d8-104">Ta je postavka široko organizacijska i kada se aktivira odmah stupa na sebi.</span><span class="sxs-lookup"><span data-stu-id="6c1d8-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="6c1d8-105">Svi uređaji koji nisu potvrđeni u sustavu Intune Server za razdoblje koje prelazi postavku trajno se brišu.</span><span class="sxs-lookup"><span data-stu-id="6c1d8-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="6c1d8-106">**Notes** Samo objekti MDM uređaja imaju pravo na ovu akciju čišćenja.</span><span class="sxs-lookup"><span data-stu-id="6c1d8-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="6c1d8-107">Ako su isključeni samo objekti uređaja.</span><span class="sxs-lookup"><span data-stu-id="6c1d8-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="6c1d8-108">Dodatne informacije o tome kada uređaj postane podoban za brisanje na temelju postavke čišćenja uređaja i njegova "stanja":</span><span class="sxs-lookup"><span data-stu-id="6c1d8-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="6c1d8-109">Postavka: **Brisanje uređaja nakon posljednjeg datuma prijave: da (neka vrijednost (N) u određenim danima)**</span><span class="sxs-lookup"><span data-stu-id="6c1d8-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="6c1d8-110">Na temelju vrijednosti (N) konfiguriranih u postavci, poslužitelj za Intune briše uređaj u navedenim danima kada se zadnji put uspješno prijavljuje.</span><span class="sxs-lookup"><span data-stu-id="6c1d8-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="6c1d8-111">Postavka:  **Brisanje uređaja nakon posljednjeg datuma prijave: ne**</span><span class="sxs-lookup"><span data-stu-id="6c1d8-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="6c1d8-112">180 dana nakon isteka certifikata uređaja i nije obnovljen, uređaj se briše.</span><span class="sxs-lookup"><span data-stu-id="6c1d8-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="6c1d8-113">**Notes** U oba slučaja uređaj mora biti uspješno registriran u programu Intune.</span><span class="sxs-lookup"><span data-stu-id="6c1d8-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="6c1d8-114">Registracija se javlja prilikom prvog provjere uređaja pomoću servisa Intune.</span><span class="sxs-lookup"><span data-stu-id="6c1d8-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="6c1d8-115">Ako se uređaj uspješno uključi, ali ne postane registriran, uređaj se briše 270 dana nakon upisa.</span><span class="sxs-lookup"><span data-stu-id="6c1d8-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="6c1d8-116">(90 dana da biste označili uređaj kao ukinut, a zatim još 180 dana da biste izbrisali zapis.)</span><span class="sxs-lookup"><span data-stu-id="6c1d8-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="6c1d8-117">U konzoli za Intune ne postoje mehanizmi za uspostavljanje datuma isteka certifikata uređaja za bilo koji uređaj.</span><span class="sxs-lookup"><span data-stu-id="6c1d8-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>