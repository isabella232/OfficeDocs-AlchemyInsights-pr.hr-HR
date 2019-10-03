---
title: Zaobilaženje predvorja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376561"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Kontrolne postavke predvorja i razina sudjelovanja

Ove postavke kontroliraju koji sudionici sastanka čekaju u predvorju prije nego što budu primljeni na sastanak i razini sudjelovanja koje su im dopuštene na sastanku. Možete koristiti PowerShell da biste ažurirali postavke pravila sastanka koje još nisu provedene (označene "uskoro") u centru za administraciju timova.  Pogledajte u nastavku za primjer PowerShell cmdlet koji omogućuje svim korisnicima da zaobiđu predvorje.  

- [Automatski priznati](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) da je osoba pravila po organizatoru koja kontrolira hoće li se ljudi izravno pridružiti sastanku ili čekati u predvorju dok ih ne primi autentizirani korisnik.

- [Dopusti anonimnim ljudima pokretanje sastanka](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je pravila po organizatoru koja kontrolira mogu li se anonimni ljudi, uključujući B2B i saveznih korisnika, pridružiti sastanku korisnika bez Autenticnog korisnika iz organizacije koja je nazočna.

- [Dopustite korisnicima biranja da zaobiđu predvorje](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira hoće li se osobe koje telefoniraju telefonom pridružiti sastanku izravno ili čekati u predvorju bez obzira na to jesu li **automatski priznali postavke korisnika** .

- [Omogućite organizatori premostiti postavke predvorja](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira može li organizator sastanka nadjačati postavke predvorja koje je administrator postavio u **automatski priznati osobe** i **dopustiti biranje korisnike da zaobiđu predvorje** kada zakazaju novi sastanak.

**Napomena:** Pročitajte [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) za potpuni pregled pravila sastanka Microsoft Teams. 


**Primjer PowerShell**

Ako želite dopustiti svima, uključujući vanjske ili anonimne korisnike, zaobići predvorje, također možete koristiti PowerShell za postizanje ovog zadatka.  Evo primjera izmjene globalne politike sastanka za vašu organizaciju.   

(Obavezno pregledajte prethodno navedenu dokumentaciju prije nego što učinite te promjene da biste razumjeli što to omogućuje.)

Set-Csteamsmetingpolicy-identitet globalni-AutoAdmittedUsers "svi"-dozvoljena Pstnuserstobypasslobby $True

Za više informacija pogledajte [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
