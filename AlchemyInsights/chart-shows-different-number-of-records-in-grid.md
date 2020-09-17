---
title: Grafikon sadrži različit broj zapisa u rešetki
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
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793750"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Grafikon sadrži različit broj zapisa u rešetki

**Simptom**

Za grafikon na stranici nadzorne ploče kada kliknete grafikon "..." i kliknite "prikaz zapisa", možete se kretati do stranice rešetke da bi vam se prikazale svi zapisi. Ponekad se broj zapisa mijenja.

**Jer**

To je zbog razlike u prikazima između grafikona na izvornoj stranici nadzorne ploče i grafikona na početnoj stranici rešetke.  

**Rješenje**

1. Provjerite prikaz s izvorne stranice i prikaza u rešetki da biste vidjeli jesu li drukčiji.
2. Promijenite prikaz u rešetki da bi odgovarao prikazu na izvornoj stranici.
3. Ako se ne pronađe ispravan prikaz, to obično znači da prikaz nije omogućen u dizajneru aplikacija.
4. Idite na dizajner aplikacije određene aplikacije, odaberite entitet i njegove prikaze, provjerite prikaz koji želite omogućiti, spremiti, objavljivati i zatvarati.
5. Osvježite stranicu.