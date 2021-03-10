---
title: Primjena najboljih postupaka za napredne lovačke upite
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692859"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Primjena najboljih postupaka za napredne lovačke upite

Da biste ubrzali rezultate i izbjegli vremenske korake tijekom izvođenja složenih upita, primijenite ove najbolje prakse:

- Prilikom pokušaja novih upita uvijek koristite ograničenje da biste izbjegli krajnje velike skupove rezultata. Upotrijebite i `count` da biste postavili početnu ocjenu veličine skupa rezultata.
- Najprije koristite filtre vremena. U idealno, ograničite upite na sedam dana.
- Na početku upita odmah nakon filtra vremena Dodajte filtre za koje se očekuje da će ukloniti većinu podataka.
- Kada tražite pune žetone, koristite operator, `has` a ne `contains` .
- Pokrenite pretraživanje na određenom stupcu, a ne u svim stupcima.
- Kada se pridružite tablicama, najprije navedite tablicu s manje redaka.
- `project` Samo potrebne stupce iz tablica kojima ste se pridružili.

Dodatne informacije potražite u članku [najbolje prakse za napredne lovačke upite](https://go.microsoft.com/fwlink/?linkid=2144812).
