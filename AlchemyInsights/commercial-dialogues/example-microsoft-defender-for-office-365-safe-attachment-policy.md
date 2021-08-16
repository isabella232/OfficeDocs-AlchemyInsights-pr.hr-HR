---
title: Example Microsoft Defender for Office 365 Sef Attachment policy
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988287"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Example Microsoft Defender for Office 365 Sef Attachment policy

Te postavke omogućuju  pravilnik bez kašnjenja koji odmah šalje poruke, a zatim ponovno šalje privitke nakon što ih skenirate:

- **Naziv**: Bez kašnjenja
- **Opis:** šalje poruke odmah i ponovno šalje privitke nakon skeniranja.
- **Odgovor**: odaberite mogućnost **Dinamička** isporuka. Dodatne informacije potražite u odjeljku [Dinamička isporuka u Sef privici](https://go.microsoft.com/fwlink/?linkid=2092328).
- **Odjeljak Za preusmjeravanje** privitka: odaberite mogućnost Omogući preusmjeravanje **,** a zatim unesite adresu e-Microsoft 365 pošte globalnog administratora, administratora sigurnosti ili sigurnosnog analitičara koji će istraživati zlonamjerne privitke.
- **Odjeljak Primijenjeno** na: **odaberite Domena primatelja** jest , a zatim odaberite domenu. Odaberite **dodaj**, a zatim U **redu**. Kada završite, odaberite **Spremi**.

Dodatne informacije potražite u članku [Sef u programu Microsoft Defender za Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
