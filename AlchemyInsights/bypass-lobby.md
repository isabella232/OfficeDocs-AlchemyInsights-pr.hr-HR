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
ms.openlocfilehash: 729fc5d4213acbbdf74a9d07adacb42b34170717
ms.sourcegitcommit: ffbeb72c9199ab4ebcb0f1ad443ed3e2f4950efc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637769"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Kontrolne postavke predvorja i razina sudjelovanja

Ako želite dopustiti svima, uključujući dial-in, vanjski i anonimni korisnici zaobići predvorje, možete koristiti PowerShell za to. Evo primjera izmjene globalne politike sastanka za vašu organizaciju:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ovaj cmdlet trenutno zahtijeva korištenje Skype za Business PowerShell modul. Da biste dobili setup koristiti ovaj cmdlet, provjerite upravljanje pravilima putem PowerShell.

Možete postaviti novo pravilo koje ćete zatim morati primijeniti na korisnike. Ako izmijenite globalnu politiku, ona će se automatski odnositi na korisnike. Za bilo koju promjenu pravila morate pričekati najmanje 4 sata i do 24 sata kako bi pravila stupile na snagu.

Obavezno pregledajte dokumentaciju u nastavku prije nego što učinite te promjene da biste razumjeli što to omogućuje.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Razumijevanje timova za sastanke u predvorju

- [Automatski priznati](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) da je osoba pravila po organizatoru koja kontrolira hoće li se ljudi izravno pridružiti sastanku ili čekati u predvorju dok ih ne primi autentizirani korisnik.

- [Dopusti anonimnim ljudima pokretanje sastanka](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je pravila po organizatoru koja kontrolira mogu li se anonimni ljudi, uključujući B2B i saveznih korisnika, pridružiti sastanku korisnika bez Autenticnog korisnika iz organizacije koja je nazočna.

- [Dopustite korisnicima biranja da zaobiđu predvorje](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira hoće li se osobe koje telefoniraju telefonom pridružiti sastanku izravno ili čekati u predvorju bez obzira na to jesu li **automatski priznali postavke korisnika** .

- [Omogućite organizatori premostiti postavke predvorja](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira može li organizator sastanka nadjačati postavke predvorja koje je administrator postavio u **automatski priznati osobe** i **dopustiti biranje korisnike da zaobiđu predvorje** kada zakazaju novi sastanak.

**Napomena:** Pročitajte [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) za potpuni pregled pravila sastanka Microsoft Teams.
