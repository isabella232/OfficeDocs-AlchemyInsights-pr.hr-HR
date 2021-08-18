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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318640"
---
# <a name="how-to-enable-hosted-voicemail"></a>Omogućivanje hostirane govorne pošte

Da biste omogućili govornu poštu, **HostedVoicemail** mora biti postavljen na $true.

Svojstvo **HostedVoicemail na** korisniku pomoću komponente Remote PowerShell (RPS).

Dodatne informacije o povezivanju s RPS-om [potražite u članku Microsoft Teams komponente PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) da biste saznali više o povezivanju s RPS-om.

1. Administrator Teams mora biti prijavljen u udaljenu ljusku PowerShell za Teams.
1. Iz naredbe PowerShell administrator Teams može pokrenuti **set-csuser user@contoso.com -HostedVoiceMail $true** gdje je sip uri korisnika o kojem je riječ.

**Napomena:** ponavljanje promjena pravilnika može potrajati do 24 sata.