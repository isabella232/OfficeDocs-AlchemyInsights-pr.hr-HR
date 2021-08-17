---
title: Upotreba DLP-a u pravilima prijenosa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084086"
---
# <a name="using-dlp-in-transport-rules"></a>Upotreba DLP-a u pravilima prijenosa

Da biste u postojeći transport integrirali sprječavanje gubitka podataka (DLP), upotrijebite uvjet „**Ako poruka sadrži...Osjetljive informacije**” u postavci pravila prijenosa.

**Dodatne detalje potražite u sljedećem članku:**

- Integrirane vrste osjetljivih informacija za DLP u pravilima prijenosa: [integriranje pravila o osjetljivim informacijama](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Pravilo ujedno možete testirati sa ili bez testa pravilnika s pomoću načina za testiranje na pravilu.  Prije testiranja biste trebali pričekati 30 minuta nakon stvaranja pravila.

- Pogledajte [Testiranje pravila tijeka/prijenosa pošte](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Napomena**: ako pokušavate implementirati novi DLP pravilnik s pravilnikom prijenosa u EAC-u, umjesto toga upotrijebite pravilnike [DLP-a u centru za sigurnost i usklađivanje](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
