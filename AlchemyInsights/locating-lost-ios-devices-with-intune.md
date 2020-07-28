---
title: Pronalaženje izgubljenih iOS uređaja s intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438906"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="e6846-102">Pronalaženje izgubljenih iOS uređaja s intune</span><span class="sxs-lookup"><span data-stu-id="e6846-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="e6846-103">Omogućivanje izgubljenog načina rada na iOS uređaju administratoru omogućuje prikaz poruke i telefonskog broja za kontakt na zaključanom zaslonu.</span><span class="sxs-lookup"><span data-stu-id="e6846-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="e6846-104">Nakon što je omogućen izgubljeni način rada, administrator može koristiti akciju Pronađi uređaj za identifikaciju fizičke lokacije uređaja.</span><span class="sxs-lookup"><span data-stu-id="e6846-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="e6846-105">Akcija Pronađi uređaj u aplikaciji Intune radi s uređajima sa sustavom iOS kako bi se prikazala lokacija određenog uređaja na karti.</span><span class="sxs-lookup"><span data-stu-id="e6846-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="e6846-106">Za korištenje ove akcije potreban je iOS uređaj:</span><span class="sxs-lookup"><span data-stu-id="e6846-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="e6846-107">Nadzirani način rada</span><span class="sxs-lookup"><span data-stu-id="e6846-107">Supervised mode</span></span>
- <span data-ttu-id="e6846-108">Način izgubljenog</span><span class="sxs-lookup"><span data-stu-id="e6846-108">Lost mode</span></span>

<span data-ttu-id="e6846-109">Dodatne informacije [potražite u odjeljku Omogućivanje izgubljenog načina rada na iOS/iPadOS uređajima s intune](https://docs.microsoft.com/intune/device-lost-mode) i [pronalaženje izgubljenih ili ukradenih iOS/iPadOS uređaja s intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="e6846-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="e6846-110">**Najčešća pitanja**</span><span class="sxs-lookup"><span data-stu-id="e6846-110">**FAQ**</span></span>

<span data-ttu-id="e6846-111">P: Izdao sam udaljenu akciju za uklanjanje podataka tvrtke s uređaja, a sada je zapela u stanju na čekanju.</span><span class="sxs-lookup"><span data-stu-id="e6846-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="e6846-112">O: Da bi se daljinsko dovršavanje uspješno dovršilo, ciljani uređaj mora biti na mreži i zdrav.</span><span class="sxs-lookup"><span data-stu-id="e6846-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="e6846-113">U sljedećim situacijama udaljena akcija ostaje u stanju na čekanju 30 dana ili dok uređaj ne potvrdi naredbu:</span><span class="sxs-lookup"><span data-stu-id="e6846-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="e6846-114">Kada uređaj nema</span><span class="sxs-lookup"><span data-stu-id="e6846-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="e6846-115">Kada uređaj izgubi status upravljanja intune</span><span class="sxs-lookup"><span data-stu-id="e6846-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="e6846-116">Ako mislite da se uređaj više ne prijavljuje i da neće moći ukloniti podatke tvrtke, odaberite Izbriši.</span><span class="sxs-lookup"><span data-stu-id="e6846-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="e6846-117">Brisanjem se uklanja zapis uređaja tako da se više ne pojavljuje na popisu Intune uređaja.</span><span class="sxs-lookup"><span data-stu-id="e6846-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="e6846-118">Ako uređaj ponovno postane aktivan, korisnik će ga morati ponovno prijaviti.</span><span class="sxs-lookup"><span data-stu-id="e6846-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="e6846-119">P: Zašto određene udaljene radnje nisu dostupne za korištenje?</span><span class="sxs-lookup"><span data-stu-id="e6846-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="e6846-120">O: Ne podržavaju sve platforme sve akcije udaljenog uređaja.</span><span class="sxs-lookup"><span data-stu-id="e6846-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="e6846-121">Sljedeće udaljene radnje specifične su za platformu, tako da su dostupne samo za navedene platforme.</span><span class="sxs-lookup"><span data-stu-id="e6846-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="e6846-122">Zaobilaženje zaključavanja aktivacije (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="e6846-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="e6846-123">Novi početak (samo windows)</span><span class="sxs-lookup"><span data-stu-id="e6846-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="e6846-124">Način izgubljenog načina rada (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="e6846-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="e6846-125">Pronalaženje uređaja (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="e6846-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="e6846-126">Ponovno pokretanje (samo windows)</span><span class="sxs-lookup"><span data-stu-id="e6846-126">Restart (Windows only)</span></span>

<span data-ttu-id="e6846-127">Dodatne pojedinosti o svakoj radnji [potražite u odjeljku Dostupne radnje uređaja](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="e6846-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>