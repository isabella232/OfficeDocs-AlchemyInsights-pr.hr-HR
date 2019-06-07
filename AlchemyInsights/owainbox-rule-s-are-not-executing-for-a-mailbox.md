---
title: 1332 OWA - Primljeno pravila se ne izvršava za poštanski sandučić
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 28b03183552e00dd2522fff51b061cc27d5032ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762215"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravilo ulazne pošte ne funkcionira prema očekivanjima

Provjerite sljedeće postavke:

- Poruku možete biti preusmjereni proslijeđene ili odgovorene automatski na temelju pravila ulazne pošte samo jednom. Preusmjeravanje pravilo (pravilo ulazne pošte ili pošte protok pravilo, poznat i kao pravilo prijevoza) možete dodati najviše deset prosljeđivanje primatelji poruke. Za dodatne informacije pogledajte [temeljnice, prijevoza, i Primljeno pravilo ograničenja](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Pravila ulazne pošte ne rade na zamjenski journaling poštanski sandučić. Dodatne informacije o journaling Alternativni poštanski sandučić pogledajte [Alternativni journaling poštanski sandučić](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Da biste riješili te probleme, pogledajte [KB 2829319](https://support.microsoft.com/kb/2829319).

Ako ne primijenite prethodne problemi, pokrenite dijagnostičkog izvješća pravilo Primljeno prije Eskaliranje problem Microsoft Support:

1. Otvoriti poštanski sandučić u programu Outlook na webu i kliknite **Postavke** \> **Mogućnosti** \> **e-pošta organiziraj** \> **pravila ulazne pošte**.

2. Na dnu stranice kliknite **Ako vaša pravila ne rade pritisnite ovdje za generiranje dijagnostičkog izvješća**.
