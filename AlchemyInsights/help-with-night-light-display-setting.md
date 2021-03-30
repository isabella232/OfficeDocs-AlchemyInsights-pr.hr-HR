---
title: Pomoć za postavku prikaza noćog svjetla
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404265"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="97257-102">Pomoć za postavku prikaza noćog svjetla</span><span class="sxs-lookup"><span data-stu-id="97257-102">Help with the night light display setting</span></span>

<span data-ttu-id="97257-103">Dodatne informacije o postavkama noćnog prikaza potražite u članku Postavljanje prikaza za [noćno vrijeme u sustavu Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="97257-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="97257-104">Ako su mogućnosti noćnog svjetla zasivljene u odjeljku Postavke, provjerite upravljački program za prikaz:</span><span class="sxs-lookup"><span data-stu-id="97257-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="97257-105">Kliknite okvir za pretraživanje na programskoj traci i upišite **Upravitelj uređaja**, a zatim u **rezultatima pretraživanja** odaberite Upravitelj uređaja.</span><span class="sxs-lookup"><span data-stu-id="97257-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="97257-106">Proširite **odjeljak Prilagodnici za prikaz**.</span><span class="sxs-lookup"><span data-stu-id="97257-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="97257-107">Značajka noćnih svjetiljki nažalost nije dostupna ako uređaj koristi upravljački program DisplayLink ili upravljački program za osnovni zaslon.</span><span class="sxs-lookup"><span data-stu-id="97257-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="97257-108">Značajka noćnog svjetla koristi nedavno korištenu grafičku tehnologiju, pa ćete možda morati ažurirati upravljački program za prikaz:</span><span class="sxs-lookup"><span data-stu-id="97257-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="97257-109">Provjerite ima li ažuriranja tako da **otvorite Start**  >  **Settings**  >  **Update & sigurnosna** provjera ažuriranja za Windows  >    >  **Update**.</span><span class="sxs-lookup"><span data-stu-id="97257-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="97257-110">OR</span><span class="sxs-lookup"><span data-stu-id="97257-110">OR</span></span>

- <span data-ttu-id="97257-111">Posjetite web-mjesto za podršku proizvođača hardvera da biste ručno preuzeli i instalirali najnovije upravljačke programe za prikaz.</span><span class="sxs-lookup"><span data-stu-id="97257-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="97257-112">Ponovno postavljanje noćnog svjetla u registru</span><span class="sxs-lookup"><span data-stu-id="97257-112">Reset night light in the registry</span></span>

<span data-ttu-id="97257-113">Ako ažuriranje upravljačkog programa za prikaz ne funkcionira, možda ćete morati ponovno postaviti noćno svjetlo u registru.</span><span class="sxs-lookup"><span data-stu-id="97257-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="97257-114">**Oprez:** Ovaj se korak za otklanjanje poteškoća preporučuje samo naprednim korisnicima.</span><span class="sxs-lookup"><span data-stu-id="97257-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="97257-115">Ako nepravilno izmijenite registar, može doći do ozbiljnih problema.</span><span class="sxs-lookup"><span data-stu-id="97257-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="97257-116">Radi dodatne zaštite sigurnosno kopiranje registra prije izmjene da biste ga mogli vratiti ako se pojave problemi.</span><span class="sxs-lookup"><span data-stu-id="97257-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="97257-117">U okvir za pretraživanje upišite **regedit**, a zatim u **rezultatima pretraživanja** odaberite Uređivač registra.</span><span class="sxs-lookup"><span data-stu-id="97257-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="97257-118">Idite na sljedeći ključ registra:</span><span class="sxs-lookup"><span data-stu-id="97257-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="97257-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="97257-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="97257-120">Izvoz i brisanje sljedećeg potključa:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="97257-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="97257-121">Izvoz i brisanje sljedećeg potključa:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="97257-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="97257-122">Ponovno pokrenite Windows i provjerite jesu li dostupne mogućnosti noćnog svjetla.</span><span class="sxs-lookup"><span data-stu-id="97257-122">Restart Windows and verify if the night light options are available.</span></span>


