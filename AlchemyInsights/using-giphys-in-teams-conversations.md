---
title: Korištenje programa Giphys u razgovorima timova
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982437"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="24af4-102">Korištenje programa Giphys u razgovorima timova</span><span class="sxs-lookup"><span data-stu-id="24af4-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="24af4-103">Pristup giphys u timovima čavrljanje omogućen je po zadanom.</span><span class="sxs-lookup"><span data-stu-id="24af4-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="24af4-104">Kao administrator možete kontrolirati jesu li Giphys dostupni korisnicima postavljanjem [pravilnika o razmjeni poruka](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) i osiguranju da je **uključeno** **Korištenje giphys u razgovorima** .</span><span class="sxs-lookup"><span data-stu-id="24af4-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="24af4-105">Ako GIF-ovi ne funkcioniraju kako se očekuje u razgovorima timova, provjerite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="24af4-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="24af4-106">[Pravilnik o razmjeni poruka](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) mora dopustiti Giphys.</span><span class="sxs-lookup"><span data-stu-id="24af4-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="24af4-107">Da biste potvrdili pomoću cmdleta u komponenti PowerShell:</span><span class="sxs-lookup"><span data-stu-id="24af4-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="24af4-108">Provjerite možete li [upravljati timovima pomoću komponente PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="24af4-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="24af4-109">Pokrenite naredbu PowerShell [Nabavite-CsTeamsMessagingPolicy – Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) i provjerite je li **Allowgiphy** postavljen na **True**.</span><span class="sxs-lookup"><span data-stu-id="24af4-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="24af4-110">Ako je **Allowgiphy** postavljen na **False** , pokrenite sljedeći skup naredbi za PowerShell [– CsTeamsMessagingPolicy – Identity Global-allowgiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="24af4-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="24af4-111">[Neobavezna povezana iskustva](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) moraju se omogućiti da bi se omogućilo pristup URL-u giphy-a.</span><span class="sxs-lookup"><span data-stu-id="24af4-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="24af4-112">Ako je za vašeg gosta konfigurirano više pravila za razmjenu poruka u timu, možete odrediti identitet pravilnika dodijeljenog korisniku koji je napravio pomoću naredbe PowerShell [Get-Csonlineuser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Odabir pravilnika TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="24af4-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
