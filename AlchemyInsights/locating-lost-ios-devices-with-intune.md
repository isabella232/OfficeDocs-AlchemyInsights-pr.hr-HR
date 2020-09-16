---
title: Pronalaženje izgubljenih uređaja sa sustavom iOS pomoću aplikacije Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675148"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="f63ae-102">Pronalaženje izgubljenih uređaja sa sustavom iOS pomoću aplikacije Intune</span><span class="sxs-lookup"><span data-stu-id="f63ae-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="f63ae-103">Omogućivanje Izgubljenog načina rada na uređaju sa sustavom iOS administrator ima poruku i telefonski broj kontakta koji se prikazuje na zaključanom zaslonu.</span><span class="sxs-lookup"><span data-stu-id="f63ae-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="f63ae-104">Nakon omogućivanja izgubljenog načina rada administrator može identificirati fizičku lokaciju uređaja pomoću akcije pronađite uređaj.</span><span class="sxs-lookup"><span data-stu-id="f63ae-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="f63ae-105">Akcija pronađite uređaj u programu Intune radi s uređajima sa sustavom iOS da bi se prikazalo mjesto određenog uređaja na karti.</span><span class="sxs-lookup"><span data-stu-id="f63ae-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="f63ae-106">Pomoću ove akcije potreban je uređaj sa sustavom iOS:</span><span class="sxs-lookup"><span data-stu-id="f63ae-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="f63ae-107">Nadzirani način rada</span><span class="sxs-lookup"><span data-stu-id="f63ae-107">Supervised mode</span></span>
- <span data-ttu-id="f63ae-108">Izgubljeni način rada</span><span class="sxs-lookup"><span data-stu-id="f63ae-108">Lost mode</span></span>

<span data-ttu-id="f63ae-109">Dodatne informacije potražite u članku [omogućivanje Izgubljenog načina rada na uređajima sa sustavom iOS/ipados pomoću aplikacije Intune](https://docs.microsoft.com/intune/device-lost-mode) i [pronalaženje izgubljenih ili ukradenih uređaja sa sustavom iOS/Ipados pomoću aplikacije Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="f63ae-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="f63ae-110">**Najčešća pitanja**</span><span class="sxs-lookup"><span data-stu-id="f63ae-110">**FAQ**</span></span>

<span data-ttu-id="f63ae-111">P: izdala sam daljinsku akciju za uklanjanje podataka tvrtke s uređaja, a sada je zaglavljena u stanju neriješenog.</span><span class="sxs-lookup"><span data-stu-id="f63ae-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="f63ae-112">O: da bi se daljinska akcija uspješno dovršena, ciljani uređaj mora biti online i zdrav.</span><span class="sxs-lookup"><span data-stu-id="f63ae-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="f63ae-113">U sljedećim situacijama daljinska akcija ostaje u stanju neriješenog tijekom 30 dana ili dok uređaj ne potvrdi naredbu:</span><span class="sxs-lookup"><span data-stu-id="f63ae-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="f63ae-114">Kada uređaj nema povezivost</span><span class="sxs-lookup"><span data-stu-id="f63ae-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="f63ae-115">Kada uređaj izgubi status upravljanja pomoću aplikacije Intune</span><span class="sxs-lookup"><span data-stu-id="f63ae-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="f63ae-116">Ako mislite da se uređaj više ne prijavljuje i da neće moći ukloniti podatke tvrtke, odaberite Izbriši.</span><span class="sxs-lookup"><span data-stu-id="f63ae-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="f63ae-117">Brisanjem se uklanja zapis uređaja tako da se više ne prikazuje na popisu Intune na uređajima.</span><span class="sxs-lookup"><span data-stu-id="f63ae-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="f63ae-118">Ako uređaj ponovno postane aktivan, njezin će ga korisnik morati ponovno prijaviti.</span><span class="sxs-lookup"><span data-stu-id="f63ae-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="f63ae-119">P: zašto određene udaljene akcije nisu dostupne za korištenje?</span><span class="sxs-lookup"><span data-stu-id="f63ae-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="f63ae-120">O: nisu sve platforme podržavaju sve akcije udaljenog uređaja.</span><span class="sxs-lookup"><span data-stu-id="f63ae-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="f63ae-121">Sljedeće udaljene akcije specifične su za platformu, pa su dostupne samo za navedene platforme.</span><span class="sxs-lookup"><span data-stu-id="f63ae-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="f63ae-122">Zaobilaženje aktivacije za aktivaciju (samo sa sustavom iOS)</span><span class="sxs-lookup"><span data-stu-id="f63ae-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="f63ae-123">Novi Start (samo u sustavu Windows)</span><span class="sxs-lookup"><span data-stu-id="f63ae-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="f63ae-124">Izgubljeni način rada (samo sa sustavom iOS)</span><span class="sxs-lookup"><span data-stu-id="f63ae-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="f63ae-125">Pronađite uređaj (samo za iOS)</span><span class="sxs-lookup"><span data-stu-id="f63ae-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="f63ae-126">Ponovno pokretanje (samo u sustavu Windows)</span><span class="sxs-lookup"><span data-stu-id="f63ae-126">Restart (Windows only)</span></span>

<span data-ttu-id="f63ae-127">Dodatne informacije o svakoj akciji potražite u članku [dostupne akcije uređaja](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="f63ae-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>