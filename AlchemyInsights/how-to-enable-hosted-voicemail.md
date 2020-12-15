---
title: Omogućivanje hostirane govorne pošte
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677028"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="08c3d-102">Omogućivanje hostirane govorne pošte</span><span class="sxs-lookup"><span data-stu-id="08c3d-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="08c3d-103">Da biste omogućili govornu poštu, **Hostedvoiemail** mora biti postavljen na $True.</span><span class="sxs-lookup"><span data-stu-id="08c3d-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="08c3d-104">Svojstvo **Hostedvoiemae** na korisniku pomoću udaljene komponente PowerShell (RPS).</span><span class="sxs-lookup"><span data-stu-id="08c3d-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="08c3d-105">Dodatne informacije o povezivanju s RPS-ovim potražite u [članku Pregled Microsoftove ekipe za PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) da biste saznali više o povezivanju s RPS-ovim.</span><span class="sxs-lookup"><span data-stu-id="08c3d-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="08c3d-106">Administrator timova trebao bi biti prijavljen u udaljenu PowerShell za timove.</span><span class="sxs-lookup"><span data-stu-id="08c3d-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="08c3d-107">Na servisu PowerShell upit administrator timova može pokrenuti **set-csuser user@contoso.com-HostedVoiceMail $True** gdje je SIP URI od korisnika koji je u pitanju.</span><span class="sxs-lookup"><span data-stu-id="08c3d-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="08c3d-108">Promjena pravilnika može potrajati i do 24 sata da bi se replicirali.</span><span class="sxs-lookup"><span data-stu-id="08c3d-108">Changes to policies can take up to 24 hours to replicate.</span></span>