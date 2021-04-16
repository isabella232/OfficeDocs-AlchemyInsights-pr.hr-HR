---
title: Rješavanje problema s Tehnologijom Bluetooth u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812924"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="db9a2-102">Rješavanje problema s Tehnologijom Bluetooth u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="db9a2-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="db9a2-103">Ako nema ikone Bluetooth ili nije moguće isključiti ili isključiti Bluetooth, pokrenite alat za otklanjanje poteškoća s Tehnologijom Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="db9a2-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="db9a2-104">[Otvorite postavke otklanjanja](ms-settings:troubleshoot)poteškoća , **u** **odjeljku Traženje i rješavanje drugih problema** kliknite Pokreni alat za otklanjanje **poteškoća**.</span><span class="sxs-lookup"><span data-stu-id="db9a2-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="db9a2-105">Ako ne vidite ikonu Bluetooth, no Bluetooth se prikazuje u upravitelju uređaja:</span><span class="sxs-lookup"><span data-stu-id="db9a2-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="db9a2-106">U upravitelju uređaja kliknite **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="db9a2-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="db9a2-107">Pritisnite i držite (ili desnom tipkom miša kliknite) naziv prilagodnika za Bluetooth pa kliknite **Deinstaliraj uređaj.**</span><span class="sxs-lookup"><span data-stu-id="db9a2-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="db9a2-108">Isključite uređaj sa sustavom Windows, pričekajte nekoliko sekundi, a zatim ga ponovno uključite.</span><span class="sxs-lookup"><span data-stu-id="db9a2-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="db9a2-109">Windows će pokušati ponovno instalirati upravljački program.</span><span class="sxs-lookup"><span data-stu-id="db9a2-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="db9a2-110">Ako ste nedavno instalirali ažuriranja sustava Windows 10 ili nadogradili na Windows 10, možda ćete trebati provjeriti ima li ažuriranja upravljačkih programa:</span><span class="sxs-lookup"><span data-stu-id="db9a2-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="db9a2-111">U upravitelju uređaja kliknite **Bluetooth**, a zatim naziv prilagodnika za Bluetooth (koji može sadržavati riječ "radio").</span><span class="sxs-lookup"><span data-stu-id="db9a2-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="db9a2-112">Pritisnite i držite (ili desnom tipkom miša kliknite) Prilagodnik za Bluetooth, a zatim automatski kliknite Ažuriraj **upravljački program**  >  **Traži ažurirani upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="db9a2-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="db9a2-113">Slijedite korake, a zatim **kliknite Zatvori**.</span><span class="sxs-lookup"><span data-stu-id="db9a2-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="db9a2-114">Ako Windows ne može pronaći novi upravljački program za Bluetooth, posjetite web-mjesto proizvođača PC-ja i preuzmite najnoviji upravljački program za Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="db9a2-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="db9a2-115">Kada ga preuzmete, kliknite Ažuriraj upravljački program Potražite upravljački program na mom računalu Potražite mjesto na kojem su datoteke upravljačkog programa pohranjene > U redu Dalje , a zatim  >    >     >  slijedite korake za instalaciju.</span><span class="sxs-lookup"><span data-stu-id="db9a2-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="db9a2-116">Nakon instalacije ažuriranog upravljačkog programa ponovno pokrenite računalo, a zatim provjerite rješava li to problem s vezom.</span><span class="sxs-lookup"><span data-stu-id="db9a2-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="db9a2-117">Dodatne informacije o otklanjanju poteškoća s Bluetoothom potražite u cjelovitom članku Rješavanje [problema s Tehnologijom Bluetooth u sustavu Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="db9a2-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
