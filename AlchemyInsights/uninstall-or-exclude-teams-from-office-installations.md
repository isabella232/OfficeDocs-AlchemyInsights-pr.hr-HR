---
title: Deinstalacija ili isključivanje aplikacije Teams iz instalacija sustava Office
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
- "2662"
- "9000660"
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827784"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="5e718-102">Deinstalacija ili isključivanje aplikacije Teams iz novih ili postojećih instalacija sustava Office</span><span class="sxs-lookup"><span data-stu-id="5e718-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="5e718-103">Microsoft Teams dio je aplikacija Microsoft 365 za velike tvrtke, aplikacija Microsoft 365 za tvrtke i sustava Office za Mac.</span><span class="sxs-lookup"><span data-stu-id="5e718-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="5e718-104">Pomoću alata [za implementaciju sustava Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) izuzimajte Teams iz novih instalacija sustava Office.</span><span class="sxs-lookup"><span data-stu-id="5e718-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="5e718-105">Da biste *deinstalirali* Teams s uređaja sa sustavom Windows, pogledajte članak [Deinstalacija aplikacije Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="5e718-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="5e718-106">Da biste microsoft Teams očistili s više ciljnih računala ili korisnika, pogledajte članak [Čišćenje implementacije aplikacije Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="5e718-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="5e718-107">Upotrijebite [mogućnost PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) da biste microsoft Teams onemogućili automatsko instaliranje sustava Office.</span><span class="sxs-lookup"><span data-stu-id="5e718-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="5e718-108">Upotrijebite [mogućnost PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) prije instalacije aplikacije *Teams* da biste spriječili automatsko pokretanje aplikacije Microsoft Teams nakon instalacije.</span><span class="sxs-lookup"><span data-stu-id="5e718-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="5e718-109">Ako koristite Office za Mac, pogledajte microsoft [Teams instalacije na Macu.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="5e718-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>