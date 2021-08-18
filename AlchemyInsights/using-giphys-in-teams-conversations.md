---
title: Korištenje značajke Giphys u Teams razgovorima
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323512"
---
# <a name="using-giphys-in-teams-conversations"></a>Korištenje značajke Giphys u Teams razgovorima

Pristup giphysu Teams čavrljanja po zadanom je omogućen. Kao administrator možete kontrolirati jesu li Giphysi [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) dostupni korisnicima postavljanjem pravilnika za razmjenu poruka i osiguravanjem da je korištenje **giphysa u razgovorima** **on**.

Ako GIF-ovi ne rade na očekivani Teams razgovora, provjerite sljedeće:

Pravilnik [za razmjenu poruka](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) mora omogućiti Giphys. Provjera pomoću cmdleta komponente PowerShell:

- Provjerite možete li upravljati [Teams komponente PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Pokrenite naredbu PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) i provjerite je **li AllowGiphy** postavljen na **TRUE**.
- Ako **je AllowGiphy** postavljen na **FALSE**, pokrenite sljedeću naredbu komponente PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Neobavezna povezana](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) sučelja moraju biti omogućena da bi se omogućio pristup URL-u giphy.

**Napomena:** ako imate više Teams za razmjenu poruka konfiguriranih za klijenta, možete odrediti identitet pravilnika dodijeljenog korisniku pomoću naredbe PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Odaberite TeamsMessagingPolicy.
