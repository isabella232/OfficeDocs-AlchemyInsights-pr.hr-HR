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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034746"
---
# <a name="fix-transport-rules"></a>Rješavanje pravila prijenosa

Prilagođeno pravilo tijeka pošte utjecalo je na ovu poruku. Da biste pregledali točno pravilo, učinite sljedeće:

1. U rezultatima slanja u **odjeljku Dodatne informacije** obratite pozornost **na GUID** ili **naziv pravilnika.**
2. Pokrenite Exchange Management Shell. Dodatne informacije potražite u članku [Otvaranje ljuske Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Pokrenite ovu naredbu (pomoću GUID-a iz slanja):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Pregledajte opis da biste vidjeli konfigurirane uvjete koji utječu na poruku.

Dodatne informacije potražite u članku [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
