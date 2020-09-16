---
title: Unos zaliha uređaja
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
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667870"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="dd087-102">Unos zaliha uređaja</span><span class="sxs-lookup"><span data-stu-id="dd087-102">Intune Device Inventory</span></span>

<span data-ttu-id="dd087-103">Oštrica uređaja sadrži administrator uvid u uređaje u odjeljku Upravljanje u programu Intune na temelju uređaja po uređaju.</span><span class="sxs-lookup"><span data-stu-id="dd087-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="dd087-104">Prikazane informacije obuhvaćaju: hardver, otkrivene aplikacije, stanje usklađenosti uređaja i stanje konfiguracije uređaja.</span><span class="sxs-lookup"><span data-stu-id="dd087-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="dd087-105">Podaci o zalihama za hardver i otkrivene aplikacije prikupljaju se sedmodnevnim ciklusom.</span><span class="sxs-lookup"><span data-stu-id="dd087-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="dd087-106">Aplikacije i posebni elementi hardvera koji su prijavljeni razlikuju se ovisno o operacijskom sustavu uređaja te je li uređaj osobno ili korporacijski vlasnik.</span><span class="sxs-lookup"><span data-stu-id="dd087-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="dd087-107">Dodatne informacije potražite u članku [Prikaz detalja o uređaju u programu Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="dd087-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="dd087-108">**Najčešća pitanja**</span><span class="sxs-lookup"><span data-stu-id="dd087-108">**FAQ**</span></span>

<span data-ttu-id="dd087-109">P: ne primam cijeli popis zaliha aplikacija prisutnih na Intune-upisanih uređaja sa sustavom Windows.</span><span class="sxs-lookup"><span data-stu-id="dd087-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="dd087-110">zašto ne?</span><span class="sxs-lookup"><span data-stu-id="dd087-110">Why not?</span></span>

<span data-ttu-id="dd087-111">O: u ovom trenutku navedene su samo moderne aplikacije za PC-jeve sa sustavom Windows 10 koje se identificiraju kao korporativni uređaji.</span><span class="sxs-lookup"><span data-stu-id="dd087-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="dd087-112">Intune ne prikuplja informacije o aplikacijama Win32 koje su instalirane na ovim uređajima.</span><span class="sxs-lookup"><span data-stu-id="dd087-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="dd087-113">P: Zašto se brojevi telefonskih brojeva ne prikupljaju na svim uređajima?</span><span class="sxs-lookup"><span data-stu-id="dd087-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="dd087-114">A: telefoni kategorizirani kao korporativni uređaji u programu Intune ne identificiraju se s punim telefonskim brojem kada, na primjer, pokrenete izvješće o zalihama mobilnog uređaja.</span><span class="sxs-lookup"><span data-stu-id="dd087-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="dd087-115">Telefonski brojevi koji donose vlastite uređaje uvijek su djelomično maskirani sa zvjezdicama (\* \* \* \*) i prikazuju samo posljednje četiri znamenke.</span><span class="sxs-lookup"><span data-stu-id="dd087-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>