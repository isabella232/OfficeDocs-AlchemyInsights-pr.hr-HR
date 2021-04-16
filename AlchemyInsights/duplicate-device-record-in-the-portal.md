---
title: Dupliciranje zapisa o uređaju na portalu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814508"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="372fc-102">Dupliciranje zapisa o uređaju na portalu</span><span class="sxs-lookup"><span data-stu-id="372fc-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="372fc-103">Možda će vam se na portalu prikazati dva zapisa o uređaju ako uređaj točno ne izvještava web-mjesto upravitelja konfiguracije o statusu zajedničkog upravljanja.</span><span class="sxs-lookup"><span data-stu-id="372fc-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="372fc-104">Da biste provjerili status zajedničkog upravljanja za uređaj, pregledajte stupac **Zajedničko upravljanje** za pripadni uređaj na konzoli programa Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="372fc-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="372fc-105">Ako stupac nije vidljiv, možete ga dodati tako da desnom tipkom miša kliknete bilo koje zaglavlje stupca i odaberete ga s popisa.</span><span class="sxs-lookup"><span data-stu-id="372fc-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="372fc-106">Vrijednost u stupcu Zajedničko upravljanje mora biti **Da**.</span><span class="sxs-lookup"><span data-stu-id="372fc-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="372fc-107">Ako je vrijednost **Ne**, otvorite klijentski aplet programa Configuration Manager i na kartici Općenito provjerite svojstvo **Zajedničko upravljanje**.</span><span class="sxs-lookup"><span data-stu-id="372fc-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="372fc-108">Ako ono ima vrijednost **Omogućeno**, to označava poteškoće s komunikacijom između klijenta i točke upravljanja.</span><span class="sxs-lookup"><span data-stu-id="372fc-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="372fc-109">Pregledajte **CcmMessaging.log** na uređaju da biste istražili moguće probleme s povezivanjem.</span><span class="sxs-lookup"><span data-stu-id="372fc-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="372fc-110">Ako svojstvo ima vrijednost **Onemogućeno**, a uređaj je prijavljen u Intune, provjerite je li uređaj primio pravilnik o zajedničkom upravljanju tako da pregledate **CoManagementHandler.log** na uređaju.</span><span class="sxs-lookup"><span data-stu-id="372fc-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
