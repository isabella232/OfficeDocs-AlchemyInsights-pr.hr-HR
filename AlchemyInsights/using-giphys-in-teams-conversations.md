---
title: Korištenje programa Giphys u razgovorima timova
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982437"
---
# <a name="using-giphys-in-teams-conversations"></a>Korištenje programa Giphys u razgovorima timova

Pristup giphys u timovima čavrljanje omogućen je po zadanom. Kao administrator možete kontrolirati jesu li Giphys dostupni korisnicima postavljanjem [pravilnika o razmjeni poruka](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) i osiguranju da je **uključeno** **Korištenje giphys u razgovorima** .

Ako GIF-ovi ne funkcioniraju kako se očekuje u razgovorima timova, provjerite sljedeće:

[Pravilnik o razmjeni poruka](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) mora dopustiti Giphys. Da biste potvrdili pomoću cmdleta u komponenti PowerShell:

- Provjerite možete li [upravljati timovima pomoću komponente PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Pokrenite naredbu PowerShell [Nabavite-CsTeamsMessagingPolicy – Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) i provjerite je li **Allowgiphy** postavljen na **True**.
- Ako je **Allowgiphy** postavljen na **False** , pokrenite sljedeći skup naredbi za PowerShell [– CsTeamsMessagingPolicy – Identity Global-allowgiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Neobavezna povezana iskustva](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) moraju se omogućiti da bi se omogućilo pristup URL-u giphy-a.

> [!NOTE]
> Ako je za vašeg gosta konfigurirano više pravila za razmjenu poruka u timu, možete odrediti identitet pravilnika dodijeljenog korisniku koji je napravio pomoću naredbe PowerShell [Get-Csonlineuser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Odabir pravilnika TeamsMessagingPolicy.
