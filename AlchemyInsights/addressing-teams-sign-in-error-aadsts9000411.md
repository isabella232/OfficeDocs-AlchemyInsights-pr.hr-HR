---
title: Rješavanje pogreške prilikom prijave timova AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357400"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Rješavanje pogreške prilikom prijave timova AADSTS9000411

Prilikom prijave u Microsoft Teams možda ćete primiti pogrešku: **Nažalost, ali imamo poteškoća s potpisivanjem u aADSTS9000411: zahtjev nije ispravno formatiran. Parametar "login_hint" je dupliciran.**

Da biste riješili taj problem, provjerite jesu li vaši klijenti sustava Microsoft Teams ažurirani. Dodatne informacije o ažuriranju klijenta potražite u [odjeljku Ažuriranje servisa Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Ako iz nekog razloga ne možete ažurirati klijenta, odjavom s klijenta izbrisat će se većina predmemorirane podatke. Međutim, ako i dalje imate problema nakon odjave/prijave, zatvorite Teams i izbrišite predmemoriju klijenta na sljedeći način:
1. Zatvorite Microsoft Teams.
2. Idite na: %appdata%\microsoft\teams i izbrišite sve datoteke.
3. Ponovno otvorite Microsoft Teams.
