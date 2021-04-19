---
title: Omogućivanje ugrađivanja naslijeđenih dijaloških okvira radi otvaranja izvješća
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814256"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Omogućivanje ugrađivanja naslijeđenih dijaloških okvira radi otvaranja izvješća

**Simptom**

Korisnici ne mogu otvarati izvješća. "Nešto nije u redu. Dodatne pojedinosti potražite u tehničkim pojedinostima."

**Uzrok**

Izvješća se ne mogu učitati u UCI uz pogrešku "Opisnik obrasca ima vrijednost null ili nije definirana". Izvješća u UCI-jem i dalje zahtijevaju naslijeđene dijaloški okvire, pa klijentov sustav mora *omogućiti omogućivo* omogućivo stvaranje sustava.

**Rješenje**

1. Otvorite **Postavke >Administracija > postavke sustava > općenito**.

2. Postavite "Enable embedding of certain legacy dialogs in Unified Interface browser client" (Omogući ugrađivanje određenih naslijeđenih dijaloških okvira u klijentu preglednika sjedinjenog sučelja) na **Da**.
