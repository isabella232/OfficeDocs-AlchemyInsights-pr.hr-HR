---
title: Upotreba DLP-a u pravilima prijenosa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915048"
---
# <a name="using-dlp-in-transport-rules"></a>Upotreba DLP-a u pravilima prijenosa

Da biste u postojeći transport integrirali sprječavanje gubitka podataka (DLP), upotrijebite uvjet „**Ako poruka sadrži...Osjetljive informacije**” u postavci pravila prijenosa.

**Dodatne detalje potražite u sljedećem članku:**

- Integrirane vrste osjetljivih informacija za DLP u pravilima prijenosa: [integriranje pravila o osjetljivim informacijama](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Pravilo ujedno možete testirati sa ili bez testa pravilnika s pomoću načina za testiranje na pravilu.  Prije testiranja biste trebali pričekati 30 minuta nakon stvaranja pravila.

- Pogledajte [Testiranje pravila tijeka/prijenosa pošte](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Napomena**: ako pokušavate implementirati novi DLP pravilnik s pravilnikom prijenosa u EAC-u, umjesto toga upotrijebite pravilnike [DLP-a u centru za sigurnost i usklađivanje](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
