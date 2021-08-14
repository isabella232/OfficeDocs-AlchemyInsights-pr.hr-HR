---
title: Adresiranje Teams pogreške prijave AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953005"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adresiranje Teams pogreške prijave AADSTS9000411

Prilikom prijave u Microsoft Teams, možda ćete primiti pogrešku: Nažalost, ali imamo problema s prijavom na **AADSTS9000411: Zahtjev nije pravilno oblikovan. Parametar "login_hint" dupliciran je.**

Da biste riješili taj problem, provjerite jesu li Microsoft Teams vaši klijenti ažurirani. Dodatne informacije o ažuriranju klijenta potražite u članku [Ažuriranje Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Ako iz nekog razloga ne možete ažurirati klijent, odjavom klijenta očistit će se većina predmemoriranog podataka. No ako i dalje imate problema nakon prijave/prijave, zatvorite Teams i očistite predmemoriju klijenta na sljedeći način:
1. Zatvorite Microsoft Teams.
2. Idite na: %appdata%\microsoft\teams i izbrišite sve datoteke.
3. Ponovno Microsoft Teams.
