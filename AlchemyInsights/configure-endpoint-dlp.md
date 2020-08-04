---
title: Konfiguriranje DLP krajnje točke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/03/2020
ms.locfileid: "46554922"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="b34a7-102">Konfiguriranje DLP krajnje točke</span><span class="sxs-lookup"><span data-stu-id="b34a7-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="b34a7-103">DLP programa Microsoft Endpoint omogućuje proširenje mogućnosti zaštite i praćenja DLP-a na osjetljive informacije na uređajima sa sustavom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="b34a7-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="b34a7-104">Nakon što se uređaji uvedu u upravljanje uređajima, možete stvoriti DLP pravila za provođenje zaštitnih akcija na stavkama.</span><span class="sxs-lookup"><span data-stu-id="b34a7-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="b34a7-105">Preglednik aktivnosti može se koristiti za nadzor aktivnosti za osjetljive stavke.</span><span class="sxs-lookup"><span data-stu-id="b34a7-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="b34a7-106">Dodatne informacije [potražite u odjeljku Uređaji za uključivanje u upravljanje uređajima](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="b34a7-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="b34a7-107">Da biste započeli s DLP-om krajnje točke:</span><span class="sxs-lookup"><span data-stu-id="b34a7-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="b34a7-108">Provjerite imate li odgovarajuće licenciranje SKU-a/pretplata.</span><span class="sxs-lookup"><span data-stu-id="b34a7-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="b34a7-109">Dodatne informacije potražite u [odjeljku Licenciranje SKU-a/pretplata](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="b34a7-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="b34a7-110">Provjerite dozvole potrebne za omogućivanje upravljanja uređajem, pristup stranici za uključivanje ili isključivanje praćenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="b34a7-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="b34a7-111">Dodatne informacije [potražite u odjeljku Dozvole](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="b34a7-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="b34a7-112">Ugrađeni uređaji u upravljanje uređajima slijedeći postupak uređaja za ukrcavanje.</span><span class="sxs-lookup"><span data-stu-id="b34a7-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="b34a7-113">Ako vam nedostaje mogućnost Uključi u ukrcaj (pretpregled) uređaja u odjeljku Postavke usklađenosti s uređajem M365 , **potvrdite**da imate gore navedenu odgovarajuću licencu i dozvole.</span><span class="sxs-lookup"><span data-stu-id="b34a7-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="b34a7-114">Dodatne informacije potražite [u odjeljku Uređaji za uključivanje .](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)</span><span class="sxs-lookup"><span data-stu-id="b34a7-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="b34a7-115">Stvorite DLP pravila da biste zaštitili osjetljive stavke.</span><span class="sxs-lookup"><span data-stu-id="b34a7-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="b34a7-116">Dodatne informacije [potražite u članku Scenariji pravila krajnjeg DLP-a](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="b34a7-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="b34a7-117">Dodatne informacije o DLP-u za Microsoft Endpoint potražite [u članku Saznajte više o sprječavanju gubitka podataka krajnje točke microsoft 365 (pretpregled).](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)</span><span class="sxs-lookup"><span data-stu-id="b34a7-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>