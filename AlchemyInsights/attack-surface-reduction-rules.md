---
title: Pravila smanjivanja površine napada
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676071"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="9d5f5-102">Pravila smanjivanja površine napada</span><span class="sxs-lookup"><span data-stu-id="9d5f5-102">Attack surface reduction rules</span></span>

<span data-ttu-id="9d5f5-103">Izuzimanje datoteka i mapa može ozbiljno smanjiti zaštitu koju pružaju pravila smanjenja površine napada.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="9d5f5-104">Datoteke koje bi pravilo blokiralo dopušteno je pokretanje i ne snima se izvješće ni događaj.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="9d5f5-105">Iznimka se primjenjuje na sva pravila koja dopuštaju izuzimanja.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="9d5f5-106">Asr izuzimanja koriste istu sintaksu kao i Microsoft Defender Antivirus izuzimanja.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="9d5f5-107">Detalje potražite u članku [Konfiguriranje i provjera valjanosti izuzimanja za Microsoft Defender Antivirus skeniranja](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="9d5f5-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="9d5f5-108">Da biste izbjegli probleme, pregledajte [uobičajene pogreške koje želite izbjeći prilikom definiranja izuzimanja.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="9d5f5-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="9d5f5-109">Ne podržavaju sva pravila ASR-a izuzimanja.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="9d5f5-110">Da biste provjerili podržava li pravilo izuzimanja, pogledajte pravila smanjenja [površine napad.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="9d5f5-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="9d5f5-111">Pravila smanjivanja površine napada</span><span class="sxs-lookup"><span data-stu-id="9d5f5-111">Attack surface reduction rules</span></span>

<span data-ttu-id="9d5f5-112">Površina za napad tvrtke ili ustanove obuhvaća sva mjesta na kojima napadač može ugroziti uređaje ili mreže tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="9d5f5-113">Smanjivanje površine napada znači zaštitu uređaja i mreže tvrtke ili ustanove, što napadačima ostavlja manje načina izvođenja napada.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="9d5f5-114">Konfiguriranje pravila smanjenja površine napada u programu Microsoft Defender za krajnju točku može vam pomoći.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="9d5f5-115">Dodatne informacije potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="9d5f5-115">For more information, see:</span></span>

- [<span data-ttu-id="9d5f5-116">Mapiranje GUID pravila ASR-a u naziv</span><span class="sxs-lookup"><span data-stu-id="9d5f5-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="9d5f5-117">Preduvjeti pravila ZA ASR:</span><span class="sxs-lookup"><span data-stu-id="9d5f5-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="9d5f5-118">Windows 10 Pro, verzija 1709 ili novija</span><span class="sxs-lookup"><span data-stu-id="9d5f5-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="9d5f5-119">Windows 10 Enterprise, verzija 1709 ili novija</span><span class="sxs-lookup"><span data-stu-id="9d5f5-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="9d5f5-120">Windows Poslužitelj, verzija 1803 (polugodišnji kanal) ili novija</span><span class="sxs-lookup"><span data-stu-id="9d5f5-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="9d5f5-121">Prepoznavanje ispravnog izuzetog sadržaja koji je moguće primijeniti</span><span class="sxs-lookup"><span data-stu-id="9d5f5-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="9d5f5-122">Potražite ID događaja 1121 ili 1122 u zapisniku microsoft-Windows-Windows Defender/Operativni zapisnik.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="9d5f5-123">Procijenite scenarij blokiranja i kontekst te potvrdite da je taj scenarij potrebno deblokirati.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="9d5f5-124">U detaljima događaja pročitajte vrijednost Put, koja je vrijednost koja definira izuzimanje.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="9d5f5-125">Izuzimanje učinite što je moguće strožim.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="9d5f5-126">Ako je potrebno, primijenite zamjenski znak (na primjer, zamijenite varijablu korisnika).</span><span class="sxs-lookup"><span data-stu-id="9d5f5-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="9d5f5-127">Primijenite izuzimanje prema potrebama implementacije.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="9d5f5-128">Detalje potražite u članku [Prilagodba pravila smanjivanja površine napada](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="9d5f5-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="9d5f5-129">Izuzimanje nije počašćeno</span><span class="sxs-lookup"><span data-stu-id="9d5f5-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="9d5f5-130">Odredite podržava li pravilo izuzimanja.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="9d5f5-131">Detalje potražite u članku Napad [pravila smanjenja površine](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="9d5f5-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="9d5f5-132">Pregledajte primijenjena izuzimanja i provjerite s podacima o događaju za pogreške ili pogrešno protumačiti zamjenske znakove.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="9d5f5-133">Dodatne informacije potražite u članku [Podržane vrste izuzimanja](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="9d5f5-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="9d5f5-134">ako je učinak pravila previsok, razmislite o premještanju pravila (natrag) u način nadzora da biste izvršili daljnju provjeru valjanosti.</span><span class="sxs-lookup"><span data-stu-id="9d5f5-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="9d5f5-135">Detalje potražite u članku [Testiranje načina na koji Microsoft Defender za značajke krajnjih točaka funkcionira u načinu rada za nadzor](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="9d5f5-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="9d5f5-136">Prikupite podatke o podršci da biste otvorili slučaj podrške pomoću ove naredbe:</span><span class="sxs-lookup"><span data-stu-id="9d5f5-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="9d5f5-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="9d5f5-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="9d5f5-138">Dodatne informacije potražite u članku [Problemi s uređajem za unošenje na Microsoft Defender za krajnje točke](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="9d5f5-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
