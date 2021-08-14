---
title: Grafikon prikazuje različit broj zapisa u rešetki
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 68ba6caf602a5cf60e2c96c80703f19dd07c3b6430c2a66f40fea4a2f3d06e75
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950072"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Grafikon prikazuje različit broj zapisa u rešetki

**Simptom**

Za grafikon na stranici nadzorne ploče kada kliknete grafikon "..." i kliknite "Prikaz zapisa", pomaknite se na stranicu rešetke da biste vidjeli sve zapise. Ponekad se broj zapisa mijenja.

**Uzrok**

To je zbog razlike u prikazima između grafikona na izvornoj stranici nadzorne ploče i grafikona na početnoj stranici rešetke.  

**Rješenje**

1. Provjerite prikaz s izvorne stranice i prikaza u rešetki da biste vidjeli razlikuju li se.
2. Promijenite prikaz u rešetki tako da odgovara prikazu na izvornoj stranici.
3. Ako nije moguće pronaći točan prikaz, to obično znači da prikaz nije omogućen u dizajneru aplikacija.
4. Idite na dizajner aplikacija određene aplikacije, odaberite entitet i njegove prikaze, provjerite prikaz koji želite omogućiti, spremiti, objaviti i zatvoriti.
5. Osvježite stranicu.