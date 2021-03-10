---
title: Rješavanje pravila prijenosa
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692824"
---
# <a name="fix-transport-rules"></a>Rješavanje pravila prijenosa

Prilagođeno pravilo tijeka e-pošte utjecalo je na ovu poruku. Da biste pregledali točno pravilo, učinite sljedeće:

1. U rezultatima slanja u odjeljku **Dodatne informacije** obratite pozornost na **GUID** ili **naziv pravilnika**.
2. Pokreni ljusku za upravljanje sustavom Exchange. Dodatne informacije potražite u članku [Otvaranje ljuske za upravljanje sustavom Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Pokretanje ove naredbe (pomoću GUID-a iz slanja):  **Nabavite-TransportRule-Identity "GUID" | FL * Opis***
4. Pregledajte Opis da biste vidjeli konfigurirane uvjete koji su utjecali na poruku.

Dodatne informacije potražite u članku [transport-Teleporttrule](https://go.microsoft.com/fwlink/?linkid=2101523).
