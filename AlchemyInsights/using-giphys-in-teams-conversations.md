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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104300"
---
# <a name="using-giphys-in-teams-conversations"></a>Korištenje značajke Giphys u Teams razgovorima

Giphys access in Teams chat is enabled by default. Kao administrator možete kontrolirati jesu li Giphysi [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) dostupni korisnicima postavljanjem pravilnika za razmjenu poruka i osiguravanjem da je korištenje **giphysa u razgovorima** **on**.

Ako GIF-ovi ne rade na očekivani Teams razgovora, provjerite sljedeće:

Pravilnik [za razmjenu poruka](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) mora omogućiti Giphys. Provjera pomoću cmdleta komponente PowerShell:

- Provjerite možete li upravljati [Teams komponente PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Pokrenite naredbu PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) i provjerite je **li AllowGiphy** postavljen na **TRUE**.
- Ako **je AllowGiphy** postavljen na **FALSE**, pokrenite sljedeću naredbu Komponente PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Neobavezna povezana](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) sučelja moraju biti omogućena da bi se omogućio pristup URL-u giphy.

> [!NOTE]
> Ako je za klijenta konfigurirano više Teams za razmjenu poruka, možete odrediti identitet pravilnika dodijeljenog korisniku pomoću naredbe PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Odaberite TeamsMessagingPolicy.
