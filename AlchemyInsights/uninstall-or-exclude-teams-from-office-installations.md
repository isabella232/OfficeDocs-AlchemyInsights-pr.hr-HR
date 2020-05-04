---
title: Deinstalacija ili izuzimanje servisa Teams iz instalacija sustava Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: b6613733e743e08a9b18b1ada70fde164b0d5dc3
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010282"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="79070-102">Deinstalacija ili izuzimanje timova iz novih ili postojećih instalacija sustava Office</span><span class="sxs-lookup"><span data-stu-id="79070-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="79070-103">Microsoft Teams dio je aplikacija Microsoft 365 za tvrtke, aplikacija sustava Microsoft 365 za tvrtke i sustava Office za Mac.</span><span class="sxs-lookup"><span data-stu-id="79070-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="79070-104">Pomoću [alata za implementaciju sustava Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) izuzmite timove iz novih instalacija sustava Office.</span><span class="sxs-lookup"><span data-stu-id="79070-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="79070-105">Da biste *instalirali* Teams s uređaja sa sustavom Windows, [pročitajte članku Deinstalacija servisa Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="79070-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="79070-106">Da biste očistili Microsoft Teams s više ciljanih računala ili korisnika, pročitajte popis [implementacije programa Microsoft Teams .](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="79070-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="79070-107">Koristite mogućnost [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) da biste spriječili automatsko instaliranje servisa Microsoft Teams pomoću sustava Office.</span><span class="sxs-lookup"><span data-stu-id="79070-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="79070-108">Koristite mogućnost [PreventFirstLaunchAfterAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) prije *instalacije timova*da biste spriječili automatsko pokretanje microsoft timova nakon instalacije.</span><span class="sxs-lookup"><span data-stu-id="79070-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="79070-109">Ako koristite Office za Mac, pročitajte upute [za Microsoft Teams na Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="79070-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>