---
title: Intune inventar uređaja
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
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438914"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="3185c-102">Intune inventar uređaja</span><span class="sxs-lookup"><span data-stu-id="3185c-102">Intune Device Inventory</span></span>

<span data-ttu-id="3185c-103">Oštrica Uređaji pruža administratorski uvid u uređaje pod upravljanjem u intuneu po uređaju.</span><span class="sxs-lookup"><span data-stu-id="3185c-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="3185c-104">Prikazane informacije uključuju: Hardver, Otkrivene aplikacije, Stanje usklađenosti uređaja i stanje konfiguracije uređaja.</span><span class="sxs-lookup"><span data-stu-id="3185c-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="3185c-105">Podaci o inventaru za hardver i otkrivene aplikacije prikupljaju se sedmodnevnim ciklusom.</span><span class="sxs-lookup"><span data-stu-id="3185c-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="3185c-106">Aplikacije i specifični elementi hardvera koji se prijavljuju razlikuju se ovisno o operacijskom sustavu uređaja i je li uređaj osobno ili u vlasništvu tvrtke.</span><span class="sxs-lookup"><span data-stu-id="3185c-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="3185c-107">Dodatne informacije [potražite u odjeljku Prikaz pojedinosti o uređaju u odjeljku Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="3185c-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="3185c-108">**Najčešća pitanja**</span><span class="sxs-lookup"><span data-stu-id="3185c-108">**FAQ**</span></span>

<span data-ttu-id="3185c-109">P: Ne primam potpuni popis inventara aplikacija prisutnih na uređajima windows koji su upisani intune.</span><span class="sxs-lookup"><span data-stu-id="3185c-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="3185c-110">Zašto ne?</span><span class="sxs-lookup"><span data-stu-id="3185c-110">Why not?</span></span>

<span data-ttu-id="3185c-111">O: Trenutno su navedene samo moderne aplikacije za PC-jeve sa sustavom Windows 10 koji su identificirani kao korporativni uređaji.</span><span class="sxs-lookup"><span data-stu-id="3185c-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="3185c-112">Intune ne prikuplja informacije o Win32 aplikacijama instaliranima na tim uređajima.</span><span class="sxs-lookup"><span data-stu-id="3185c-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="3185c-113">P: Zašto se telefonski brojevi ne prikupljaju sa svih uređaja?</span><span class="sxs-lookup"><span data-stu-id="3185c-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="3185c-114">O: Telefoni kategorizirani kao korporativni uređaji u tvrtki Intune ne identificiraju se s punim telefonskim brojem kada, na primjer, pokrenete izvješće o inventaru mobilnih uređaja.</span><span class="sxs-lookup"><span data-stu-id="3185c-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="3185c-115">Bring-you-vlastiti uređaj telefonski brojevi su uvijek djelomično maskirani sa zvjezdicama (\*\*\*\*), i pokazati samo posljednje četiri znamenke.</span><span class="sxs-lookup"><span data-stu-id="3185c-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>