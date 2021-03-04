---
title: Uključivanje nadzora poštanskog sandučića
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429287"
---
# <a name="turn-on-mailbox-auditing"></a>Uključivanje nadzora poštanskog sandučića

Da biste uključili nadzor poštanskog sandučića za jednog korisnika ili cijelu tvrtku ili ustanovu, pokrenite sljedeće cmdlete iz udaljene komponente PowerShell:

- **Jednostruki korisnik**: Set-Mailbox-Identity "Jane Dow" – auditenabled $True
- **Tvrtka ili ustanova**: Get-Mailbox-Rezultsize neograničeno-filtar {RecipientTypeDetails-aq "UserMailbox"} | Set-Mailbox $true

Dodatne informacije potražite u članku [Upravljanje nadziranje poštanskog sandučića](https://go.microsoft.com/fwlink/?linkid=2103668).