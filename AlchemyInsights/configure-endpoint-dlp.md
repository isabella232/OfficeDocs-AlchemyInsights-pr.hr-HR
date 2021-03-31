---
title: Konfiguriranje DLP-a u krajnjim točkama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402407"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="0278c-102">Konfiguriranje DLP-a u krajnjim točkama</span><span class="sxs-lookup"><span data-stu-id="0278c-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="0278c-103">Microsoftov DLP u krajnjim točkama omogućuje proširenje mogućnosti zaštite DLP-a i sposobnosti nadzora osjetljivih podataka na uređajima sa sustavom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="0278c-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="0278c-104">Kada se uređaji umetnu u upravljanje uređajima, možete stvoriti pravilnike o DLP-u da biste primijenili zaštitni radnje za stavke.</span><span class="sxs-lookup"><span data-stu-id="0278c-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="0278c-105">Eksplorer za aktivnosti može se upotrebljavati za praćenje aktivnosti povjerljivih stavki.</span><span class="sxs-lookup"><span data-stu-id="0278c-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="0278c-106">Dodatne informacije potražite u odjeljku [Uvođenje uređaja u upravljanje uređajima](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="0278c-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="0278c-107">Početak rada s DLP-om u krajnjim točkama:</span><span class="sxs-lookup"><span data-stu-id="0278c-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="0278c-108">Provjerite imate li odgovarajuću licencu za SKU/pretplate.</span><span class="sxs-lookup"><span data-stu-id="0278c-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="0278c-109">Dodatne informacije potražite u članku [Licenciranje za SKU/pretplate](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="0278c-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="0278c-110">Provjerite dozvole potrebne za omogućivanje upravljanja uređajima, pristup stranici za uvođenje ili uključivanje/isključivanje nadzora uređaja.</span><span class="sxs-lookup"><span data-stu-id="0278c-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="0278c-111">Dodatne informacije potražite u članku [Dozvole](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="0278c-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="0278c-112">Uvedite uređaje u upravljanje uređajima s pomoću postupka za uvođenje uređaja.</span><span class="sxs-lookup"><span data-stu-id="0278c-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="0278c-113">Ako ne možete odabrati mogućnost uvođenja uređaja (pretpregled) u odjeljku **Postavke** usklađenosti za M365, provjerite imate li gore navedene odgovarajuće licence i dozvole.</span><span class="sxs-lookup"><span data-stu-id="0278c-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="0278c-114">Dodatne informacije potražite u članku [Uvođenje uređaja](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="0278c-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="0278c-115">Stvorite pravilnike o DLP-u radi zaštite osjetljivih stavki.</span><span class="sxs-lookup"><span data-stu-id="0278c-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="0278c-116">Dodatne informacije potražite u [scenarijima pravilnika DLP-a za krajnje točke](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="0278c-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="0278c-117">Dodatne informacije o Microsoftovom DLP-u za krajnje točke potražite u članku [Dodatne informacije o sprječavanju gubitka podataka krajnjih točaka u sustavu Microsoft 365 (pretpregled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="0278c-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="0278c-118">**Važni koraci za prikupljanje podataka, ako je potrebna podrška:**</span><span class="sxs-lookup"><span data-stu-id="0278c-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="0278c-119">Preuzimanje pretpregleda MDATP alata za analizu klijenta iz sustava [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="0278c-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="0278c-120">Pokrenite alat kao administrator iz prozora cmd:</span><span class="sxs-lookup"><span data-stu-id="0278c-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="0278c-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="0278c-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="0278c-122">Kada se pojavi upit „Unesite broj minuta za prikupljanje praćenja: ”, unesite broj minuta potrebnih za pokretanje scenarija</span><span class="sxs-lookup"><span data-stu-id="0278c-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="0278c-123">Pokretanje scenarija</span><span class="sxs-lookup"><span data-stu-id="0278c-123">Run the scenario</span></span>

<span data-ttu-id="0278c-124">Prikupite izlaznu zip datoteku koja će se dati agentu za podršku.</span><span class="sxs-lookup"><span data-stu-id="0278c-124">Collect the Zip file output to be given to the Support agent.</span></span>
