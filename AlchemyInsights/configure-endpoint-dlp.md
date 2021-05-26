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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657921"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="03baa-102">Konfiguriranje DLP-a u krajnjim točkama</span><span class="sxs-lookup"><span data-stu-id="03baa-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="03baa-103">Microsoftov DLP u krajnjim točkama omogućuje proširenje mogućnosti zaštite DLP-a i sposobnosti nadzora osjetljivih podataka na uređajima sa sustavom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="03baa-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="03baa-104">Kada se uređaji umetnu u upravljanje uređajima, možete stvoriti pravilnike o DLP-u da biste primijenili zaštitni radnje za stavke.</span><span class="sxs-lookup"><span data-stu-id="03baa-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="03baa-105">Eksplorer za aktivnosti može se upotrebljavati za praćenje aktivnosti povjerljivih stavki.</span><span class="sxs-lookup"><span data-stu-id="03baa-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="03baa-106">Dodatne informacije potražite u odjeljku [Uvođenje uređaja u upravljanje uređajima](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="03baa-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="03baa-107">Početak rada s DLP-om u krajnjim točkama:</span><span class="sxs-lookup"><span data-stu-id="03baa-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="03baa-108">Provjerite imate li odgovarajuću licencu za SKU/pretplate.</span><span class="sxs-lookup"><span data-stu-id="03baa-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="03baa-109">Dodatne informacije potražite u članku [Licenciranje za SKU/pretplate](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="03baa-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="03baa-110">Provjerite dozvole potrebne za omogućivanje upravljanja uređajima, pristup stranici za uvođenje ili uključivanje/isključivanje nadzora uređaja.</span><span class="sxs-lookup"><span data-stu-id="03baa-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="03baa-111">Dodatne informacije potražite u članku [Dozvole](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="03baa-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="03baa-112">Uvedite uređaje u upravljanje uređajima s pomoću postupka za uvođenje uređaja.</span><span class="sxs-lookup"><span data-stu-id="03baa-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="03baa-113">Dodatne informacije potražite u članku [Uvođenje uređaja](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="03baa-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="03baa-114">Stvorite pravilnike o DLP-u radi zaštite osjetljivih stavki.</span><span class="sxs-lookup"><span data-stu-id="03baa-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="03baa-115">Dodatne informacije potražite u [scenarijima pravilnika DLP-a za krajnje točke](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="03baa-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="03baa-116">Dodatne informacije o Microsoftovom DLP-u za krajnje točke potražite u članku [Dodatne informacije o sprječavanju gubitka podataka krajnjih točaka u sustavu Microsoft 365 (pretpregled)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="03baa-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="03baa-117">**Važni koraci za prikupljanje podataka, ako je potrebna podrška:**</span><span class="sxs-lookup"><span data-stu-id="03baa-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="03baa-118">Preuzimanje [pretpregleda alata za analizu klijenta za MDATP](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="03baa-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="03baa-119">Pokrenite alat kao administrator iz prozora cmd:</span><span class="sxs-lookup"><span data-stu-id="03baa-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="03baa-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="03baa-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="03baa-121">Kada se od vas zatraži **da unesete broj minuta** za prikupljanje praćenja: unesite broj minuta potrebnih za pokretanje scenarija.</span><span class="sxs-lookup"><span data-stu-id="03baa-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="03baa-122">Pokrenite scenarij.</span><span class="sxs-lookup"><span data-stu-id="03baa-122">Run the scenario.</span></span>

<span data-ttu-id="03baa-123">Prikupite izlaz zip datoteke koji želite dati agentu za podršku.</span><span class="sxs-lookup"><span data-stu-id="03baa-123">Collect the Zip file output to give to the Support agent.</span></span>
