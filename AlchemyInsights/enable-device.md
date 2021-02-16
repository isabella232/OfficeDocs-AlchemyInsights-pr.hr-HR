---
title: Omogućivanje uređaja
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
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256706"
---
# <a name="enable-device"></a>Omogućivanje uređaja

**Omogućivanje uređaja pomoću naredbe PowerShell**

Pokrenite sljedeće naredbe:

- Da biste dohvatili objekt uređaja: `Get-MsolDevice -Name <Name>`
- Da biste omogućili uređaj, učinite sljedeće: `Enable-MsolDevice -DeviceId <DeviceId>`

Dodatne informacije o konfiguriranju hibridnog pridruživanja na upravljanim domenama potražite u članku [Konfiguriranje hibridna pridruživanja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
