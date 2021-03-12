---
title: Primjeri pravilnika o privitku programa Microsoft Defender za Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743677"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Primjeri pravilnika o privitku programa Microsoft Defender za Office 365

Ove postavke omogućuju pravilo koje se zove *nema kašnjenja* koje odmah dostavljaju poruke, a zatim ponovno prilaže privitke nakon skeniranja:

- **Naziv**: nema kašnjenja
- **Opis**: odmah dostavlja poruke i ponovno prilaže privitke nakon skeniranja.
- **Odgovor**: odaberite mogućnost **dinamičke isporuke** . Dodatne informacije potražite u članku [dinamička isporuka u pravilima sigurnog privitaka](https://go.microsoft.com/fwlink/?linkid=2092328).
- Odjeljak **preusmjeravanje privitaka** : odaberite mogućnost **Omogućivanje preusmjeravanja**, a zatim unesite adresu e-pošte sustava Microsoft 365 Global administrator, administrator sigurnosti ili sigurnosni analitičar koji će istraživati zlonamjerne privitke.
- **Primijenjena na** sekciju: odaberite **domenu primatelja**, a zatim odaberite svoju domenu. Odaberite **Dodaj**, a zatim odaberite **u redu**. Kada završite, odaberite **Spremi**.

Dodatne informacije potražite u članku [sigurni privici u programu Microsoft Defender za Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
