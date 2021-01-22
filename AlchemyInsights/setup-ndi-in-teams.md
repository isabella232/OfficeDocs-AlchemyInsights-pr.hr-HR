---
title: Uključivanje NDI tehnologije
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
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935075"
---
# <a name="turn-on-ndi-technology"></a>Uključivanje NDI tehnologije

Za NDI tehnologiju potrebna su dva koraka koja će biti uključena za korisnika:

1. Administrator korisnika mora omogućiti svojstvo "AllowNDIStreaming" u odjeljku CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Kada se ta promjena popunjava, krajnji korisnik mora uključiti NDI® tehnologiju za određene klijente iz **postavki > dozvola**.

Dodatne informacije potražite u članku [Korištenje NDI tehnologije u Microsoftovim timovima](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
