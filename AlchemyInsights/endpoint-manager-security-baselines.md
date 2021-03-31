---
title: EndPoint Manager – polazišta za sigurnost
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440870"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="ae8cc-102">EndPoint Manager – polazišta za sigurnost</span><span class="sxs-lookup"><span data-stu-id="ae8cc-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="ae8cc-103">Polazišta za sigurnost unaprijed su konfigurirane grupe postavki sustava Windows koje vam pomažu primijeniti sigurnosne postavke koje preporučuju nadležni timovi zaduženi za sigurnost.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="ae8cc-104">Ta se polazišta mogu prilagoditi kako bi se provele samo željene postavke i vrijednosti.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="ae8cc-105">Da biste saznali više informacija o polazištima za sigurnost, pročitajte članak [Upotreba polazišta za sigurnost za konfiguriranje uređaja sa sustavom Windows 10 u sustavu Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="ae8cc-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="ae8cc-106">Trenutačno postoje polazišta za ove proizvode:</span><span class="sxs-lookup"><span data-stu-id="ae8cc-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="ae8cc-107">Sigurnosne postavke za Windows MDM</span><span class="sxs-lookup"><span data-stu-id="ae8cc-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="ae8cc-108">Sigurnost za Microsoft Defender za krajnju točku</span><span class="sxs-lookup"><span data-stu-id="ae8cc-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="ae8cc-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ae8cc-109">Microsoft Edge</span></span>

<span data-ttu-id="ae8cc-110">Svako od polazišta redovito se ažurira i izdaje u postupnim verzijama.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="ae8cc-111">Svaka verzija dodaje i/ili uklanja postavke iz prethodnih verzija kako bi se osiguralo da to polazište bude u skladu s trenutačnim smjernicama.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="ae8cc-112">Konzola Polazišta za sigurnost u Sigurnosti krajnje točke omogućuje usporedbu različitih verzija tako što se promjene iz jedne verzije u drugu čine vidljivima.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="ae8cc-113">Da biste saznali smjernice o tome kako najučinkovitije promijeniti koja se verzija polazišta implementira, pročitajte članak [Upravljanje profilima polazišta za sigurnost u sustavu Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="ae8cc-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="ae8cc-114">Nakon provedbe polazišta za sigurnost možete nadzirati stanje provedbe i pregledavati postavke za svaki uređaj zasebno.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="ae8cc-115">**Napomena:** kod podataka o izvješćivanju za polazišta mogu proteći do 24 sata prije no što oni budu vidljivi nakon prve provedbe na uređaju i do 6 sati za daljnja ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="ae8cc-116">Najčešći uzrok za to da se određena postavka polazišta ne primjenjuje jest taj što istu postavku upotrebljava drugi profil.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="ae8cc-117">Ovaj se scenarij može istražiti za svaki uređaj tako što će se taj uređaj odabrati iz čvora Stanje uređaja profila Polazište za sigurnost.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="ae8cc-118">Da biste saznali pojedinosti, pročitajte članak [Rješavanje sukoba za polazišta za sigurnost](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="ae8cc-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>