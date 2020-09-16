---
title: Rješavanje problema s tehnologijom Bluetooth u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730151"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="76ef1-102">Rješavanje problema s tehnologijom Bluetooth u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="76ef1-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="76ef1-103">Ako nema ikone Bluetooth ili Bluetooth nije moguće uključiti ili isključiti, možda ćete htjeti pokrenuti alat za otklanjanje poteškoća s Bluetooth-om.</span><span class="sxs-lookup"><span data-stu-id="76ef1-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="76ef1-104">[Otvorite postavke otklanjanja poteškoća](ms-settings:troubleshoot), kliknite **Bluetooth** da biste **pronašli i riješili druge probleme**, kliknite **Pokreni alat za otklanjanje poteškoća**.</span><span class="sxs-lookup"><span data-stu-id="76ef1-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="76ef1-105">Ako vam se ne prikazuje ikona Bluetootha, no Bluetooth se prikazuje u upravitelju uređaja:</span><span class="sxs-lookup"><span data-stu-id="76ef1-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="76ef1-106">U upravitelju uređaja kliknite **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="76ef1-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="76ef1-107">Pritisnite i držite (ili kliknite desnom tipkom miša) naziv Bluetooth prilagodnika, a zatim kliknite **Deinstaliraj uređaj**.</span><span class="sxs-lookup"><span data-stu-id="76ef1-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="76ef1-108">Isključite uređaj sa sustavom Windows, pričekajte nekoliko sekundi, a zatim ga ponovno uključite.</span><span class="sxs-lookup"><span data-stu-id="76ef1-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="76ef1-109">Windows će pokušati ponovno instalirati upravljački program.</span><span class="sxs-lookup"><span data-stu-id="76ef1-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="76ef1-110">Ako ste nedavno instalirali ažuriranja za Windows 10 ili nadogradili na Windows 10, zatražite ažuriranja upravljačkih programa:</span><span class="sxs-lookup"><span data-stu-id="76ef1-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="76ef1-111">U upravitelju uređaja kliknite **Bluetooth**, a zatim kliknite naziv Bluetooth prilagodnika (koji može uključivati riječ "radio").</span><span class="sxs-lookup"><span data-stu-id="76ef1-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="76ef1-112">Pritisnite i držite (ili desnom tipkom miša kliknite) Bluetooth prilagodnik, a zatim kliknite **Ažuriranje upravljačkog programa**  >  **automatskog pretraživanja radi ažuriranog upravljačkog**programa.</span><span class="sxs-lookup"><span data-stu-id="76ef1-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="76ef1-113">Slijedite korake, a zatim kliknite **Zatvori**.</span><span class="sxs-lookup"><span data-stu-id="76ef1-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="76ef1-114">Ako Windows ne može pronaći novi upravljački program za Bluetooth, posjetite web-mjesto proizvođača PC-ja i preuzmite najnoviji upravljački program za Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="76ef1-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="76ef1-115">Kada ga preuzmete, kliknite **Ažuriraj upravljački program**  >  **Pregledaj moje računalo da**biste potražili upravljački program  >  **Browse** za mjesto na kojem su spremljene datoteke upravljačkog programa > **u redu**  >  **dalje**, a zatim slijedite korake koje želite instalirati.</span><span class="sxs-lookup"><span data-stu-id="76ef1-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="76ef1-116">Nakon instalacije ažuriranog upravljačkog programa ponovno pokrenite uređaj, a zatim provjerite rješava li to problem s vezom.</span><span class="sxs-lookup"><span data-stu-id="76ef1-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="76ef1-117">Dodatne informacije o otklanjanju poteškoća s Bluetooth vezom potražite u članku cijeli članak i [otklanjanje problema s Bluetooth programom u sustavu Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="76ef1-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
