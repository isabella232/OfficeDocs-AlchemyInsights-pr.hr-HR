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
# <a name="how-to-enable-hosted-voicemail"></a>Omogućivanje hostirane govorne pošte

Da biste omogućili govornu poštu, **Hostedvoiemail** mora biti postavljen na $True.

Svojstvo **Hostedvoiemae** na korisniku pomoću udaljene komponente PowerShell (RPS).

Dodatne informacije o povezivanju s RPS-ovim potražite u [članku Pregled Microsoftove ekipe za PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) da biste saznali više o povezivanju s RPS-ovim.

1. Administrator timova trebao bi biti prijavljen u udaljenu PowerShell za timove.
1. Na servisu PowerShell upit administrator timova može pokrenuti **set-csuser user@contoso.com-HostedVoiceMail $True** gdje je SIP URI od korisnika koji je u pitanju.

> [!NOTE]
> Promjena pravilnika može potrajati i do 24 sata da bi se replicirali.