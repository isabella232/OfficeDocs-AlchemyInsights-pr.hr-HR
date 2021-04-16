---
title: Odgađanje nadogradnje aplikacije Teams
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
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801223"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="884f7-102">Odgađanje nadogradnje aplikacije Microsoft-driven Teams</span><span class="sxs-lookup"><span data-stu-id="884f7-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="884f7-103">**Važno**: To vam možemo pomoći riješiti pomoću dijagnostičke podrške, ali čini se da ne koristite Novi centar za administratore.</span><span class="sxs-lookup"><span data-stu-id="884f7-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="884f7-104">Da biste koristili novi centar za administratore, pomaknite prekidač u gornjem desnom desnoj tipki u koji piše **novi centar za administratore** desno.</span><span class="sxs-lookup"><span data-stu-id="884f7-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="884f7-105">Pomoću novog centra za administratore kliknite widget Potrebna **vam je pomoć?** upišite "Odgodi nadogradnju aplikacije Teams", a zatim slijedite upute za pokretanje dijagnostike.</span><span class="sxs-lookup"><span data-stu-id="884f7-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="884f7-106">Ako ste primili komunikaciju o microsoftovoj automatiziranoj nadogradnji sa servisa Skype za tvrtke na Microsoft Teams i želite odgoditi automatiziranu nadogradnju na kasniji datum, globalni administrator može se prijaviti na portal administratora aplikacije [Teams,](https://admin.teams.microsoft.com/dashboard) a nakon odabira **gumba Status** osvježavanja u odjeljku Nadogradnja aplikacije Microsoft Teams odaberite gumb **Odgodi.**</span><span class="sxs-lookup"><span data-stu-id="884f7-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="884f7-107">Da biste vidjeli novi datum automatske nadogradnje klijenta na Microsoft Teams, osvježite stranicu portala Za administratore aplikacije Teams.</span><span class="sxs-lookup"><span data-stu-id="884f7-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="884f7-108">**Napomena:** Gumb **Odgodi** bit će dostupan samo ako ste primili obavijest centra za poruke o automatiziranoj nadogradnji.</span><span class="sxs-lookup"><span data-stu-id="884f7-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="884f7-109">Globalni administratori mogu pokrenuti i [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) da bi saznali više o trenutnom statusu nadogradnje.</span><span class="sxs-lookup"><span data-stu-id="884f7-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
