---
title: Rješavanje problema s prijavom u timove za AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687030"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Rješavanje problema s prijavom u timove za AADSTS9000411

Kada se prijavite u Microsoftove timove, možda će vam se prikazati pogreška: Žao nam je **, ali imamo problema s prijavom u AADSTS9000411: zahtjev nije pravilno oblikovan. Parametar "login_hint" dupliciran je.**

Da biste riješili taj problem, provjerite ažuriraju li se klijenti Microsoftova timova. Dodatne informacije o ažuriranju klijenta potražite u članku [Ažuriranje Microsoftovih timova](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Ako ne možete ažurirati klijenta iz nekog razloga, odprijavite se od klijenta koji će izbrisati većinu predmemoriranih podataka. No ako i dalje imate problema nakon odjave/prijave, napustite timove i poništite svoj klijent predmemorija na sljedeći način:
1. Zatvaranje Microsoftovih timova.
2. Idite na:%AppData%\microsoft\timovi i izbrišite sve datoteke.
3. Ponovno otvorite Microsoftove timove.
