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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055546"
---
# <a name="how-to-enable-hosted-voicemail"></a>Omogućivanje hostirane govorne pošte

Da biste omogućili govornu poštu, **HostedVoicemail** mora biti postavljen na $true.

Svojstvo **HostedVoicemail na** korisniku pomoću komponente Remote PowerShell (RPS).

Dodatne informacije o povezivanju s RPS-om potražite u članku Microsoft Teams pregled ljuske [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) da biste saznali više o povezivanju s RPS-om.

1. Administrator Teams mora biti prijavljen u udaljenu ljusku PowerShell za Teams.
1. U dodatku PowerShell administrator Teams može pokrenuti **set-csuser user@contoso.com -HostedVoiceMail $true** gdje je sip uri korisnika o kojem je riječ.

> [!NOTE]
> Ponavljanje promjena pravilnika može potrajati i do 24 sata.