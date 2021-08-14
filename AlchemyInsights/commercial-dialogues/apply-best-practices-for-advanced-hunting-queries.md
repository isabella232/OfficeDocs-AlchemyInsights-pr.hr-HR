---
title: Primjena najboljih praksi za napredne upite o lovanju
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930125"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Primjena najboljih praksi za napredne upite o lovanju

Da biste brže dobili rezultate i izbjegli timeouts tijekom pokretanja složenih upita, primijenite sljedeće najbolje prakse:

- Prilikom pokušaja novih upita uvijek koristite ograničenje da biste izbjegli dobivanje vrlo velikih skupova rezultata. Uz `count` to, koristite se za početnu procjenu veličine skupa rezultata.
- Najprije upotrijebite vremenske filtre. U idealnom su redu da upite ograničite na sedam dana.
- Na početku upita odmah nakon filtra vremena dodajte filtre za koje se očekuje da će ukloniti većinu podataka.
- Kada tražite pune tokene, koristite operator umjesto `has` `contains` .
- Pokrenite pretraživanje na određenom stupcu umjesto u svim stupcima.
- Prilikom pridruživanja tablicama najprije navedite tablicu s manje redaka.
- `project` samo potrebne stupce iz tablica koje ste pridružili.

Dodatne informacije potražite u članku [Napredne prakse lovačkog upita](https://go.microsoft.com/fwlink/?linkid=2144812).
