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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003381"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Omogućivanje ugrađivanja naslijeđenih dijaloških okvira radi otvaranja izvješća

**Simptom**

Korisnici ne mogu otvarati izvješća. "Nešto nije u redu. Dodatne pojedinosti potražite u tehničkim pojedinostima."

**Uzrok**

Izvješća se ne mogu učitati u UCI uz pogrešku "Opisnik obrasca ima vrijednost null ili nije definirana". Izvješća u UCI-jem i dalje zahtijevaju naslijeđene dijaloški okvire, pa klijentov sustav mora *omogućiti omogućivo* omogućivo stvaranje sustava.

**Rješenje**

1. Idite **na Postavke >Administratorski > System Postavke > Općenito kartica**.

2. Postavite "Enable embedding of certain legacy dialogs in Unified Interface browser client" (Omogući ugrađivanje određenih naslijeđenih dijaloških okvira u klijentu preglednika sjedinjenog sučelja) na **Da**.
