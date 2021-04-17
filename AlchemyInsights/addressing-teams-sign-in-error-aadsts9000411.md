---
title: Pogreška prilikom prijave u Teams AADSTS9000411
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
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821979"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Pogreška prilikom prijave u Teams AADSTS9000411

Prilikom prijave u Microsoft Teams može vam se prikazati pogreška: Nažalost, ali imamo problema s prijavom u **AADSTS9000411: Zahtjev nije pravilno oblikovan. Parametar "login_hint" dupliciran je.**

Da biste riješili taj problem, provjerite ažuriraju li se klijenti servisa Microsoft Teams. Dodatne informacije o ažuriranju klijenta potražite u članku Ažuriranje [aplikacije Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Ako iz nekog razloga ne možete ažurirati klijent, odjavom klijenta očistit će se većina predmemoriranog podataka. No ako i dalje imate problema nakon prijave/prijave, zatvorite Teams i očistite predmemoriju klijenta na sljedeći način:
1. Zatvorite Microsoft Teams.
2. Idite na: %appdata%\microsoft\teams i izbrišite sve datoteke.
3. Ponovno otvorite Microsoft Teams.
