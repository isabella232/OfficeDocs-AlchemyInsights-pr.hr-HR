---
title: Rješavanje problema s Bluetoothom u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268590"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="27956-102">Rješavanje problema s Bluetoothom u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="27956-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="27956-103">Ako ikona Bluetooth nedostaje ili Bluetooth ne može biti uključen ili isključen, možda želite pokrenuti alat za otklanjanje poteškoća s Bluetoothom.</span><span class="sxs-lookup"><span data-stu-id="27956-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="27956-104">[Otvorite postavke otklanjanja poteškoća](ms-settings:troubleshoot), kliknite **Bluetooth** u odjeljku **Traženje i rješavanje drugih problema**, kliknite Pokreni alat za otklanjanje **poteškoća**.</span><span class="sxs-lookup"><span data-stu-id="27956-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="27956-105">Ako ne vidite ikonu Bluetooth, ali Bluetooth se pojavljuje u upravitelju uređaja:</span><span class="sxs-lookup"><span data-stu-id="27956-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="27956-106">U upravitelju uređaja kliknite **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="27956-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="27956-107">Pritisnite i držite (ili kliknite desnom tipkom miša) naziv Bluetooth prilagodnika i kliknite **Deinstaliraj uređaj**.</span><span class="sxs-lookup"><span data-stu-id="27956-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="27956-108">Isključite uređaj sa sustavom Windows, pričekajte nekoliko sekundi, a zatim ga ponovno uključite.</span><span class="sxs-lookup"><span data-stu-id="27956-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="27956-109">Windows će pokušati ponovno instalirati upravljački program.</span><span class="sxs-lookup"><span data-stu-id="27956-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="27956-110">Ako ste nedavno instalirali ažuriranja za Windows 10 ili nadogradili na Windows 10, možda ćete htjeti provjeriti ima li ažuriranja upravljačkih programa:</span><span class="sxs-lookup"><span data-stu-id="27956-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="27956-111">U upravitelju uređaja kliknite **Bluetooth**, a zatim naziv Bluetooth prilagodnika (koji može sadržavati riječ "radio").</span><span class="sxs-lookup"><span data-stu-id="27956-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="27956-112">Pritisnite i držite (ili kliknite desnom tipkom miša) Bluetooth prilagodnik, a zatim kliknite **Ažuriraj upravljački program** > **Automatski traži ažurirani upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="27956-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="27956-113">Slijedite korake, a zatim kliknite **Zatvori**.</span><span class="sxs-lookup"><span data-stu-id="27956-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="27956-114">Ako Windows ne može pronaći novi upravljački program za Bluetooth, posjetite web-mjesto proizvođača PC-ja i odatle preuzmite najnoviji Upravljački program za Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="27956-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="27956-115">Nakon što ga preuzmete, kliknite **Ažuriraj upravljački program** > Potražite upravljački program > na**mom računalu Potražite**mjesto na kojem su datoteke upravljačkog programa pohranjene > U **redu** > **Dalje**i slijedite korake koje želite instalirati.\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="27956-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="27956-116">Nakon instalacije ažuriranog upravljačkog programa ponovno pokrenite računalo, a zatim provjerite je li to riješilo problem s vezom.</span><span class="sxs-lookup"><span data-stu-id="27956-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="27956-117">Dodatne pojedinosti o otklanjanju poteškoća s Bluetooth om potražite u cijelom članku, [Riješite probleme s Bluetoothom u sustavu Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="27956-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
