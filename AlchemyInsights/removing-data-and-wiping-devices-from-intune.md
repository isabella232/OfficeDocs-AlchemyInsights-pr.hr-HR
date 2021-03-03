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
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416305"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="2be8f-102">Uklanjanje podataka i brisanje uređaja iz programa Intune</span><span class="sxs-lookup"><span data-stu-id="2be8f-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="2be8f-103">Uređaj se povlači, a uređaj briše udaljene akcije, može se koristiti za uklanjanje podataka tvrtke koje upravlja Intune ili za izvođenje tvornice i vraćanje uređaja na zadane postavke.</span><span class="sxs-lookup"><span data-stu-id="2be8f-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="2be8f-104">Prijavite se u upravljanje uređajima Microsoft 365, a zatim otvorite **Uređaji**  >  **Svi uređaji**.</span><span class="sxs-lookup"><span data-stu-id="2be8f-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="2be8f-105">Odaberite uređaj koji želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="2be8f-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="2be8f-106">Odaberite vrstu daljinskog brisanja koju želite učiniti.</span><span class="sxs-lookup"><span data-stu-id="2be8f-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="2be8f-107">Povlačenje briše samo organizacijske podatke, dok pune maramice vraćaju uređaj na tvorničke postavke.</span><span class="sxs-lookup"><span data-stu-id="2be8f-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="2be8f-108">Odaberite **da** da biste potvrdili.</span><span class="sxs-lookup"><span data-stu-id="2be8f-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="2be8f-109">Dok brisanje ne završi, status akcije uređaja prikazuje se kao *umirovljen na čekanju*.</span><span class="sxs-lookup"><span data-stu-id="2be8f-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="2be8f-110">Nakon dovršetka akcije više nećete vidjeti mobilni uređaj na popisu upravljanog uređaja.</span><span class="sxs-lookup"><span data-stu-id="2be8f-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="2be8f-111">Podaci o poduzeću ne mogu se ukloniti s uređaja koji su spojeni na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2be8f-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="2be8f-112">Informacije o efektu umirovljenja i brisanja, uključujući ono što je sačuvano i izbrisano, potražite u članku sljedeća dokumentacija:</span><span class="sxs-lookup"><span data-stu-id="2be8f-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="2be8f-113">[Uklonite uređaje pomoću značajke brisanje, povlačenje ili ručno poništavanje upisivanjem uređaja](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="2be8f-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="2be8f-114">Brisanje samo korporativnih podataka iz aplikacija koje upravlja Intune</span><span class="sxs-lookup"><span data-stu-id="2be8f-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="2be8f-115">[Brisanje svih podataka s macOS uređaja](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="2be8f-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>