---
title: Uklanjanje podataka i brisanje uređaja iz intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438913"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="d2a77-102">Uklanjanje podataka i brisanje uređaja iz intune</span><span class="sxs-lookup"><span data-stu-id="d2a77-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="d2a77-103">Daljinske akcije za povlačenje uređaja i brisanje uređaja mogu se koristiti za uklanjanje podataka tvrtke kojima upravlja Intune ili za vraćanje na tvorničke postavke i vraćanje uređaja na zadane postavke.</span><span class="sxs-lookup"><span data-stu-id="d2a77-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="d2a77-104">Prijavite se u Microsoft 365 Device Management i idite na **Uređaji**  >  **svi uređaji**.</span><span class="sxs-lookup"><span data-stu-id="d2a77-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="d2a77-105">Odaberite uređaj koji želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="d2a77-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="d2a77-106">Odaberite vrstu daljinskog brisanja koju želite učiniti.</span><span class="sxs-lookup"><span data-stu-id="d2a77-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="d2a77-107">Povlačenjem se brišu samo organizacijske informacije, dok potpuno brisanje vraća uređaj na tvorničke postavke.</span><span class="sxs-lookup"><span data-stu-id="d2a77-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="d2a77-108">Odaberite **Da** za potvrdu.</span><span class="sxs-lookup"><span data-stu-id="d2a77-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="d2a77-109">Dok brisanje ne završi, status akcije Uređaja prikazuje se kao Neriješeno.</span><span class="sxs-lookup"><span data-stu-id="d2a77-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="d2a77-110">Nakon dovršetka akcije mobilni uređaj više nećete vidjeti na popisu upravljanih uređaja.</span><span class="sxs-lookup"><span data-stu-id="d2a77-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="d2a77-111">**Napomena:** Podaci tvrtke ne mogu se ukloniti s uređaja pridruženih azure AD.</span><span class="sxs-lookup"><span data-stu-id="d2a77-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="d2a77-112">Potpune pojedinosti o učinku akcija "Umirovljenje i brisanje" u svrhu povlačenja i brisanja potražite u [odjeljku Uklanjanje uređaja brisanjem, povlačenjem ili ručnim uklanjanjem uređaja](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="d2a77-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="d2a77-113">Da biste izbrisali sve podatke s macOS uređaja, pročitajte pravila [Brisanje svih podataka s macOS uređaja](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="d2a77-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>