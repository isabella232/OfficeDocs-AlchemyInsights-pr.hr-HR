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
# <a name="private-channels-in-microsoft-teams"></a>Privatni kanali u aplikaciji Microsoft Teams

Privatni kanali nova su značajka u aplikaciji Microsoft Teams. Imajte na umu da se privatni kanali ne mogu pretvoriti iz standardnih kanala ili obrnuto.

Pojedinosti o privatnim kanalima, kao što su informacije o [stvaranju privatnih kanala, članstvu](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) i [privatnim web-mjestima sustava SharePoint,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)potražite u članku [Privatni kanali u sustavu Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Napomena:** Budući da konfiguracija zadržavanja privatnih poruka kanala još nije podržana, klijenti s omogućenim pravilima zadržavanja prema zadanim postavkama neće imati omogućene privatne kanale. Privatni kanali mogu se omogućiti u centru za administratore timova. Također, imajte na umu da iako zadržavanje privatnih poruka kanala nije podržano, podržano je zadržavanje datoteka koje se zajednički koriste u privatnim kanalima.

**Trebate novog vlasnika tima?**

Ako vaš vlasnik privatnog kanala napusti, možete dodati novog vlasnika tima putem komponente Teams Powershell.


- Idite [ovdje](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) da biste instalirali Teams Powershell.

Ovdje je cmdlet koji će vam trebati:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Dodatne informacije o programu Teams Powershell potražite u članku [Pregled komponente Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
