---
title: EndPoint Manager – sigurnosne osnovne vrijednosti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420719"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="36a3f-102">EndPoint Manager – sigurnosne osnovne vrijednosti</span><span class="sxs-lookup"><span data-stu-id="36a3f-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="36a3f-103">Sigurnosne su osnovne vrijednosti unaprijed konfigurirane grupe postavki sustava Windows koje vam pomažu pri primjeni sigurnosnih postavki koje preporučuju odgovarajući sigurnosni timovi.</span><span class="sxs-lookup"><span data-stu-id="36a3f-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="36a3f-104">Te se osnovne vrijednosti mogu prilagoditi tako da se isporučuju samo željene postavke i vrijednosti.</span><span class="sxs-lookup"><span data-stu-id="36a3f-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="36a3f-105">Dodatne informacije o sigurnosnim osnovnim vrijednostima potražite u članku Konfiguriranje uređaja sa sustavom [Windows 10 pomoću sigurnosnih osnova u aplikaciji Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="36a3f-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="36a3f-106">Trenutno postoje osnovne vrijednosti za ove proizvode:</span><span class="sxs-lookup"><span data-stu-id="36a3f-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="36a3f-107">Postavke sigurnosti MDM-a u sustavu Windows</span><span class="sxs-lookup"><span data-stu-id="36a3f-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="36a3f-108">Microsoft Defender for EndPoint Security</span><span class="sxs-lookup"><span data-stu-id="36a3f-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="36a3f-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="36a3f-109">Microsoft Edge</span></span>

<span data-ttu-id="36a3f-110">Svaka od osnovnih vrijednosti ažurira se povremeno i ispušta u inkrementalnim verzijama.</span><span class="sxs-lookup"><span data-stu-id="36a3f-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="36a3f-111">Svaka verzija dodaje i uklanja postavke iz prethodne verzije da bi osnovna vrijednost zadovoljavala trenutne smjernice.</span><span class="sxs-lookup"><span data-stu-id="36a3f-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="36a3f-112">Konzola Sigurnosne osnovne vrijednosti u sigurnosti krajnjih točaka omogućuje uspoređenje različitih verzija tako da se promjene iz verzije u verziju uspoređuju vidljivima.</span><span class="sxs-lookup"><span data-stu-id="36a3f-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="36a3f-113">Upute za učinkovitu promjenu verzije osnovne vrijednosti potražite u članku Upravljanje sigurnosnim osnovnim [profilima u aplikaciji Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="36a3f-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="36a3f-114">Nakon implementacije sigurnosne osnovice možete pratiti stanje implementacije i pregledati postavke na temelju uređaja po uređaj.</span><span class="sxs-lookup"><span data-stu-id="36a3f-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="36a3f-115">**Napomena:** Podaci za izvješćivanje o osnovnim vrijednostima mogu potrajati do 24 sata da bi se pojavili od početne implementacije na uređaj i do 6 sati radi dodatnih ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="36a3f-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="36a3f-116">Najčešći uzrok ne primjenjuje se osnovna postavka jer se ista postavka koristi u drugom profilu.</span><span class="sxs-lookup"><span data-stu-id="36a3f-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="36a3f-117">Taj se scenarij može istražiti za određeni uređaj tako da odaberete taj uređaj u sklopu sustava Status uređaja profila sigurnosne osnovice.</span><span class="sxs-lookup"><span data-stu-id="36a3f-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="36a3f-118">Detalje potražite u članku [Razrješavanje sukoba za sigurnosne osnovne vrijednosti](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="36a3f-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>