---
title: Hodnik za zaobilaženje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684942"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Upravljanje postavkama predvorja i razinom sudjelovanja u timovima

Ako želite dopustiti svima, uključujući biranjem, vanjskim i anonimnim korisnicima, **zaobići predvorje**, pomoću komponente PowerShell možete izvršiti ovaj zadatak. Evo primjera izmjene pravilnika globalnog sastanka za vašu tvrtku ili ustanovu.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ovaj cmdlet trenutno zahtijeva korištenje modula za Skype za tvrtke PowerShell. Da biste se postavili za korištenje tog cmdleta, pogledajte [Upravljanje pravilima pomoću komponente PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Kada postavite pravilnik, morate ga primijeniti na korisnike; Ako ste izmijenili globalno pravilo, ona će se automatski primijeniti na korisnike. Za bilo koju promjenu pravila morate čekati najmanje **4 sata do 24 sata** da bi pravila stupila na utjecaj. 

Obavezno pregledajte dokumentaciju u nastavku prije nego što ove promjene razumijete točno što to omogućuje.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Upravljanje pravilima predvorja za sastanke s timovima

Te postavke kontroliraju sudionike sastanka koji čekaju u predvorju prije nego što ih prime na sastanak i na razinu sudjelovanja koje im je dopušteno na sastanku. Pomoću komponente PowerShell možete ažurirati postavke pravilnika sastanka koje još nisu implementirane (s oznakom "uskoro") u centru za administratore timova. U nastavku potražite ogledni cmdlet za PowerShell koji korisnicima omogućuje zaobilaženje predvorja.

- [Automatski Priznajte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) da su korisnici po pravilima organizatora koji kontroliraju hoće li se osobe izravno pridružiti sastanku ili čekati u predvorju dok ih ne prizna ovjereni korisnik.

- [Dopuštanje anonimnih osoba da pokrene sastanak](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) jest pravilo po organizatoru koje kontrolira jesu li anonimni osobe, uključujući B2B i udruženu korisnike, mogli sudjelovati u sastanku korisnika bez ovlaštenog korisnika iz tvrtke ili ustanove.

- [Dopusti korisnicima biranjem zaobilaženje predvorja](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira hoće li se osobe koje se biraju putem telefona izravno pridružiti sastanku ili čekati u predvorju bez obzira na to da **automatski priznaju postavljanje osoba** .

- [Dopusti organizatorima da nadjačaju postavke predvorja](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**uskoro**) predstavlja pravilnik o organizatoru koja kontrolira može li organizator sastanka nadjačati postavke predvorja koje je administrator postavio **automatski priznaje osobe** i **Dopusti korisnicima biranjem zaobilaženje predvorja** prilikom zakazivanja novog sastanka.

**Upozorenje:** Pročitajte [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) za potpuni pregled pravilnika o sastanku u Microsoftovim timovima.
