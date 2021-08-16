---
title: Uključivanje tehnologije NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023514"
---
# <a name="turn-on-ndi-technology"></a>Uključivanje tehnologije NDI

Za NDI tehnologiju potrebno je uključili dva koraka za korisnika:

1. Administrator klijenta mora omogućiti svojstvo "AllowNDIStreaming" u programu CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Kada se ta promjena popuni, krajnji korisnik mora uključiti NDI® tehnologiju za određeni klijent iz **Postavke > dozvole**.

Dodatne informacije potražite u članku [Korištenje tehnologije NDI u sustavu Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
