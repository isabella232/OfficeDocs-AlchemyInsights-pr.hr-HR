---
title: Zaobići potaknuće zaključati na nadzirani iOS sprava sa Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423367"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="d6613-102">Zaobići potaknuće zaključati na nadzirani iOS sprava sa Intune</span><span class="sxs-lookup"><span data-stu-id="d6613-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="d6613-103">Mogućnost zaobilaženja zaključavanja aktivacije na iOS uređajima olakšava oporavak od scenarija u kojem korisnik omogućuje zaključavanje aktivacije na korporativnom uređaju, a zatim napušta tvrtku.</span><span class="sxs-lookup"><span data-stu-id="d6613-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="d6613-104">Preduvjeti za zaobilaženje zaključavanja aktivacije uključuju:</span><span class="sxs-lookup"><span data-stu-id="d6613-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="d6613-105">Uređaj je da je "pod nadzorom."</span><span class="sxs-lookup"><span data-stu-id="d6613-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="d6613-106">Zaključavanje aktivacije uspješno je omogućeno pomoću pravila ograničenja iOS uređaja u sustavu Intune.</span><span class="sxs-lookup"><span data-stu-id="d6613-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="d6613-107">Osim toga, prilikom zaobilaženja zaključavanja aktivacije trebali biste:</span><span class="sxs-lookup"><span data-stu-id="d6613-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="d6613-108">Fizički posjedujete uređaj koji se briše.</span><span class="sxs-lookup"><span data-stu-id="d6613-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="d6613-109">Kopirajte kôd prije nego što izdate brisanje.</span><span class="sxs-lookup"><span data-stu-id="d6613-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="d6613-110">**Napomena:** Kôd za brisanje ne razlikuje velika i mala slova, pa znakovi "-" nisu potrebni.</span><span class="sxs-lookup"><span data-stu-id="d6613-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="d6613-111">Pojedinosti potražite [u odjeljku Zaobilaženje zaključavanja aktivacije na nadziranim iOS uređajima pomoću mogućnosti Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="d6613-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="d6613-112">**Najčešća pitanja**</span><span class="sxs-lookup"><span data-stu-id="d6613-112">**FAQ**</span></span>

<span data-ttu-id="d6613-113">P: **Izdao sam udaljenu akciju za uklanjanje podataka tvrtke s uređaja, a sada je zapela u stanju na čekanju.**</span><span class="sxs-lookup"><span data-stu-id="d6613-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="d6613-114">O: Da bi se daljinsko dovršavanje uspješno dovršilo, ciljani uređaj mora biti na mreži i zdrav.</span><span class="sxs-lookup"><span data-stu-id="d6613-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="d6613-115">U sljedećim situacijama udaljena akcija ostaje u stanju na čekanju 30 dana ili dok uređaj ne potvrdi naredbu kada uređaj:</span><span class="sxs-lookup"><span data-stu-id="d6613-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="d6613-116">Nema veze.</span><span class="sxs-lookup"><span data-stu-id="d6613-116">Does not have connectivity.</span></span>
- <span data-ttu-id="d6613-117">Gubi svoj status upravljanja s Intune.</span><span class="sxs-lookup"><span data-stu-id="d6613-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="d6613-118">Ako mislite da se uređaj više ne prijavljuje i da neće ukloniti podatke tvrtke, odaberite Izbriši.</span><span class="sxs-lookup"><span data-stu-id="d6613-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="d6613-119">Brisanjem se uklanja zapis uređaja tako da se više ne pojavljuje na popisu Intune uređaja.</span><span class="sxs-lookup"><span data-stu-id="d6613-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="d6613-120">Da bi uređaj ponovno postao aktivan, njegov korisnik mora ponovno prijaviti uređaj.</span><span class="sxs-lookup"><span data-stu-id="d6613-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="d6613-121">P: **Zašto određene udaljene radnje nisu dostupne za korištenje?**</span><span class="sxs-lookup"><span data-stu-id="d6613-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="d6613-122">O: Ne podržavaju sve platforme sve akcije udaljenog uređaja.</span><span class="sxs-lookup"><span data-stu-id="d6613-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="d6613-123">Sljedeće udaljene radnje specifične su za platformu.</span><span class="sxs-lookup"><span data-stu-id="d6613-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="d6613-124">Zaobilaženje zaključavanja aktivacije (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="d6613-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="d6613-125">Novi početak (samo windows)</span><span class="sxs-lookup"><span data-stu-id="d6613-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="d6613-126">Način izgubljenog načina rada (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="d6613-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="d6613-127">Pronalaženje uređaja (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="d6613-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="d6613-128">Ponovno pokretanje (samo windows)</span><span class="sxs-lookup"><span data-stu-id="d6613-128">Restart (Windows only)</span></span>

<span data-ttu-id="d6613-129">Dodatne pojedinosti o svakoj radnji [potražite u odjeljku Dostupne radnje uređaja](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="d6613-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>