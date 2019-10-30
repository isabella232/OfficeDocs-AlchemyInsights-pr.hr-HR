---
title: Deinstaliranje ili isključivanje timova iz Officeovih instalacija
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
ms.openlocfilehash: c6d5c0233acb8fb71127dcb54c719b71aa1a5bcb
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769799"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="90767-102">Deinstaliranje ili isključivanje timova iz novih ili postojećih instalacija sustava Office</span><span class="sxs-lookup"><span data-stu-id="90767-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="90767-103">Microsoft Teams uključen je u sklopu sustava Office 365 ProPlus, Office 365 Business i Office za Mac.</span><span class="sxs-lookup"><span data-stu-id="90767-103">Microsoft Teams is included as part of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span>

- <span data-ttu-id="90767-104">Pomoću [alata za implementaciju sustava Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) isključite timove iz novih instalacija sustava Office.</span><span class="sxs-lookup"><span data-stu-id="90767-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="90767-105">Da biste *deinstalirali* timove s uređaja sa sustavom Windows, pogledajte [Deinstaliraj Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="90767-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="90767-106">Da biste počistili Microsoftove timove iz višestrukih ciljnih strojeva ili korisnika, pogledajte [Postavljanje programa Microsoft Teams za čišćenje](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="90767-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="90767-107">Koristite mogućnost [Preventteamsinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) da biste spriječili Microsoft Teams da automatski instaliraju Office.</span><span class="sxs-lookup"><span data-stu-id="90767-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="90767-108">Upotrijebite mogućnost [Preventfirstlaunchafterinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , *prije nego što timovi budu instalirani*, kako bi spriječili automatsko pokretanje programa Microsoft Teams nakon instalacije.</span><span class="sxs-lookup"><span data-stu-id="90767-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="90767-109">Ako koristite Office za Mac, pogledajte [instalacije Microsoft Teams na Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="90767-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>