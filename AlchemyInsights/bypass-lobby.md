---
title: Zaobilazno predvorje
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059588"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Upravljanje postavkama predvorja i razinom sudjelovanja u Teams

Ako želite omogućiti svima, uključujući uključivanje biranjem, vanjske i anonimne korisnike, da zaobilaze predvorje, upotrijebite PowerShell da biste izvršili taj zadatak. Evo primjera izmjene pravilnika globalnog sastanka za vašu organizaciju.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ovaj cmdlet trenutno zahtijeva korištenje modula Skype za tvrtke PowerShell. Da biste se postavili za korištenje ovog cmdleta, pogledajte upravljanje [pravilnikom putem komponente PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Kada postavite pravilnik, morate ga primijeniti na korisnike. ili, ako ste izmijenili globalni pravilnik, on će se automatski primijeniti na korisnike. Da bi se pravila mijenjala, morate pričekati najmanje **4 sata do 24 sata da** bi pravila snazi. 

Obavezno pregledajte dokumentaciju u nastavku da biste točno razumjeli što to omogućuje.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Objašnjenje Teams kontrola pravilnika u predvorju sastanka

Te postavke kontroliraju sudionike sastanka koji čekaju u predvorju prije nego što se prihvate na sastanak i razinu sudjelovanja koja im je dopuštena u sastanku. PowerShell možete koristiti za ažuriranje postavki pravilnika sastanka koje još nisu implementirane (označene kao "uskoro") u centru Teams administratora. U nastavku pogledajte primjer cmdleta Komponente PowerShell koji svim korisnicima omogućuje zaobilaženje predvorja.

- [Automatsko priznanje osoba](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) pravilnik je po organizatoru koji određuje hoće li se osobe izravno uključiti u sastanak ili čekati u predvorju dok ih korisnik ne primi.

- [Omogući anonimnim osobama](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) da započinju sastanak pravilnik je po organizatoru koji određuje mogu li se anonimne osobe, uključujući B2B i združene korisnike, uključiti u korisnikov sastanak bez provjere autentičnosti korisnika iz tvrtke ili ustanove.

- [Omogući korisnicima uključivanje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) biranjem da zaobilaze predvorje **(uskoro**) pravilnik je po organizatoru koji određuje hoće li se osobe koje se pozivaju telefonom izravno uključiti u sastanak ili čekati u predvorju bez obzira na postavku Automatski **priznaj osobe.**

- [Dopusti organizatorima da nadjačaju](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) postavke predvorja (uskoro ) pravilnik je po organizatoru koji  određuje može li organizator sastanka nadjačati postavke predvorja koje je postavio administrator u odjeljku Automatski prima osobe i Dopusti korisnicima za uključivanje **biranjem** da zaobilaze predvorje kada zakaže novi sastanak.

**Napomena:** Pročitajte [upravljanje pravilnikom za Teams za](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) potpuni pregled pravilnika Microsoft Teams sastanaka.
