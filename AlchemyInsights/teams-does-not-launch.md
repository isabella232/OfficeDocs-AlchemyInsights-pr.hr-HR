---
title: Teams se ne pokreće
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813342"
---
# <a name="teams-doesnt-launch"></a>Teams se ne pokreće

Ako pokušate otvoriti Microsoft Teams, ali se nikad ne pokreće, pokušajte sljedeće:

1. Pronađite **%appdata%\Microsoft\Teams**.
1. Izbrišite sadržaj mape.
1. Ponovno pokrenite računalo i pokušajte pokrenuti Teams.

Možda ćete morati ponovno instalirati Teams. Ponovna instalacija:

1. Deinstalirajte Teams pomoću upravljačke ploče.
1. Pronađite **%appdata%\Microsoft\Teams\Application Cache**.
1. Izbrišite sadržaj mape.
1. Pronađite **%appdata%\Microsoft\teams\Cache**.
1. Izbrišite sadržaj mape.
1. Ponovno pokrenite računalo, a zatim preuzmite i instalirajte Teams.

Ako želite pokrenuti dijagnostiku na klijentu za određenog korisnika koji se ne može prijaviti, pokrenite novo pretraživanje pomoću ključne **riječi TeamsUserUnableToSignIn** i slijedite upute.