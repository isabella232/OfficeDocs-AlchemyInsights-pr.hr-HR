---
title: Privatni kanal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005430"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="7e2fd-102">Privatni kanali u aplikaciji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7e2fd-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="7e2fd-103">Privatni kanali nova su značajka u aplikaciji Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7e2fd-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="7e2fd-104">Imajte na umu da se privatni kanali ne mogu pretvoriti iz standardnih kanala ili obrnuto.</span><span class="sxs-lookup"><span data-stu-id="7e2fd-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="7e2fd-105">Pojedinosti o privatnim kanalima, kao što su informacije o [stvaranju privatnih kanala, članstvu](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) i [privatnim web-mjestima sustava SharePoint,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)potražite u članku [Privatni kanali u sustavu Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="7e2fd-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="7e2fd-106">**Napomena:** Budući da konfiguracija zadržavanja privatnih poruka kanala još nije podržana, klijenti s omogućenim pravilima zadržavanja prema zadanim postavkama neće imati omogućene privatne kanale.</span><span class="sxs-lookup"><span data-stu-id="7e2fd-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="7e2fd-107">Privatni kanali mogu se omogućiti u centru za administratore timova.</span><span class="sxs-lookup"><span data-stu-id="7e2fd-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="7e2fd-108">Također, imajte na umu da iako zadržavanje privatnih poruka kanala nije podržano, podržano je zadržavanje datoteka koje se zajednički koriste u privatnim kanalima.</span><span class="sxs-lookup"><span data-stu-id="7e2fd-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="7e2fd-109">**Trebate novog vlasnika tima?**</span><span class="sxs-lookup"><span data-stu-id="7e2fd-109">**Need a new team owner?**</span></span>

<span data-ttu-id="7e2fd-110">Ako vaš vlasnik privatnog kanala napusti, možete dodati novog vlasnika tima putem komponente Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="7e2fd-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="7e2fd-111">Idite [ovdje](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) da biste instalirali Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="7e2fd-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="7e2fd-112">Ovdje je cmdlet koji će vam trebati:</span><span class="sxs-lookup"><span data-stu-id="7e2fd-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="7e2fd-113">Dodatne informacije o programu Teams Powershell potražite u članku [Pregled komponente Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="7e2fd-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
