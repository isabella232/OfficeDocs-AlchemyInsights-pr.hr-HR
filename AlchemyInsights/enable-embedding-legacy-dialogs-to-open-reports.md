---
title: Omogućivanje otvaranja naslijeđenih dijaloga ugradnjom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: ca0894849e95fd69acd2065c3f065547231a07f9
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204652"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Omogućivanje otvaranja naslijeđenih dijaloga ugradnjom

**Simptom**

Korisnici ne mogu otvoriti izvješća. "Nešto je pošlo po zlu. Provjerite tehničke detalje za više detalja."

**Uzrokovati**

Izvješća se ne učitavaju u UCI s pogreškom "Opisnik obrasca je null ili nije definiran." Izvješća u UCI-ju i dalje zahtijevaju naslijeđene dijaloge, tako da klijentov sustav mora omogućiti omogućeno *nasljeđivanje dijagnoze.*

**Rješenje**

1. Idite na **karticu Postavke >administracije > postavke sustava > Općenito**.

2. Postavite "Omogući ugrađivanje određenih naslijeđenih dijaloga u klijentu preglednika objedinjenog sučelja" na **Da**.
