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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889074"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrolne postavke predvorja i razina sudjelovanja u timovima

Ako želite dopustiti svima, uključujući dial-in, vanjski i anonimni korisnici, **zaobići predvorje**, koristite PowerShell za postizanje ovog zadatka. Evo primjera izmjene globalne politike sastanka za vašu organizaciju.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ovaj cmdlet trenutno zahtijeva korištenje Skype za Business PowerShell modul. Da biste dobili postavljen za korištenje ovog cmdlet, provjerite [Upravljanje pravilima putem PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Nakon što postavite pravilo, morate ga primijeniti na korisnike; ili, ako ste izmijenili globalnu politiku, ona će se automatski odnositi na korisnike. Za bilo koju promjenu pravila morate pričekati najmanje **4 sata do 24 sata** kako bi pravila stupile na snagu. 

Obavezno pregledajte dokumentaciju u nastavku prije nego što učinite te promjene da biste razumjeli što to omogućuje.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Razumijevanje timova za sastanke u predvorju

Ove postavke kontroliraju koji sudionici sastanka čekaju u predvorju prije nego što budu primljeni na sastanak i razini sudjelovanja koje su im dopuštene na sastanku. Možete koristiti PowerShell da biste ažurirali postavke pravila sastanka koje još nisu provedene (označene "uskoro") u centru za administraciju timova. Pogledajte u nastavku za primjer PowerShell cmdlet koji omogućuje svim korisnicima da zaobiđu predvorje.

- [Automatski priznati](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) da je osoba pravila po organizatoru koja kontrolira hoće li se ljudi izravno pridružiti sastanku ili čekati u predvorju dok ih ne primi autentizirani korisnik.

- [Dopusti anonimnim ljudima pokretanje sastanka](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je pravila po organizatoru koja kontrolira mogu li se anonimni ljudi, uključujući B2B i saveznih korisnika, pridružiti sastanku korisnika bez Autenticnog korisnika iz organizacije koja je nazočna.

- [Dopustite korisnicima biranja da zaobiđu predvorje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira hoće li se osobe koje telefoniraju telefonom pridružiti sastanku izravno ili čekati u predvorju bez obzira na to jesu li **automatski priznali postavke korisnika** .

- [Omogućite organizatori nadjačati postavke predvorja](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira može li organizator sastanka nadjačati postavke predvorja koje je administrator postavio u **automatski priznati ljude** i **dopustiti dial-in korisnicima da zaobiđu predvorje** kada zakazaju novi sastanak.

**Napomena:** Pročitajte [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) za potpuni pregled pravila sastanka Microsoft Teams.
