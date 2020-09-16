---
title: Uklanjanje podataka i brisanje uređaja iz programa Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701275"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="89db7-102">Uklanjanje podataka i brisanje uređaja iz programa Intune</span><span class="sxs-lookup"><span data-stu-id="89db7-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="89db7-103">Uređaj se povlači, a uređaj briše udaljene akcije, može se koristiti za uklanjanje podataka tvrtke koje upravlja Intune ili za izvođenje tvornice i vraćanje uređaja na zadane postavke.</span><span class="sxs-lookup"><span data-stu-id="89db7-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="89db7-104">Prijavite se u upravljanje uređajima Microsoft 365, a zatim otvorite **Uređaji**  >  **Svi uređaji**.</span><span class="sxs-lookup"><span data-stu-id="89db7-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="89db7-105">Odaberite uređaj koji želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="89db7-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="89db7-106">Odaberite vrstu daljinskog brisanja koju želite učiniti.</span><span class="sxs-lookup"><span data-stu-id="89db7-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="89db7-107">Povlačenje briše samo organizacijske podatke, dok pune maramice vraćaju uređaj na tvorničke postavke.</span><span class="sxs-lookup"><span data-stu-id="89db7-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="89db7-108">Odaberite **da** da biste potvrdili.</span><span class="sxs-lookup"><span data-stu-id="89db7-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="89db7-109">Dok brisanje ne završi, status akcije uređaja prikazuje se kao umirovljen na čekanju.</span><span class="sxs-lookup"><span data-stu-id="89db7-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="89db7-110">Nakon dovršetka akcije više nećete vidjeti mobilni uređaj na popisu upravljanog uređaja.</span><span class="sxs-lookup"><span data-stu-id="89db7-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="89db7-111">**Notes** Podaci o poduzeću ne mogu se ukloniti s uređaja koji su spojeni na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="89db7-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="89db7-112">Sve pojedinosti o efektu umirovljenja i brisanja akcije, uključujući ono što je sačuvano i izbrisane, potražite u članku [uklanjanje uređaja pomoću značajke brisanja, umirovljenja ili ručnog brisanja uređaja](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="89db7-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="89db7-113">Da biste izbrisali sve podatke s macOS uređaja, pročitajte članak [Brisanje svih podataka s MacOS uređaja](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="89db7-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>