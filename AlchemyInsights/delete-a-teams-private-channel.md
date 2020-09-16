---
title: Brisanje privatnog kanala timova
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730907"
---
# <a name="delete-a-teams-private-channel"></a>Brisanje privatnog kanala timova

Microsoft je svjestan problema s brisanjem privatnog kanala timova ako su pravila zadržavanja sustava SharePoint omogućena za web-mjesto sustava SharePoint u podlozi. Microsoft radi na ispravcima. U međuvremenu možete izbrisati privatni kanal pomoću sljedećih zaobilaznih rješenja.

**Izuzimanje tima/zbirke web-mjesta iz pravilnika o zadržavanju sustava SharePoint.**

1. Idite na portal za administratore sustava Office 365, a zatim odaberite **Prikaz svih** u lijevoj navigacijskom oknu.
2. U odjeljku **centri za administratore**idite na **Sigurnosno &**  >  pravilnik o**sprječavanju gubitka podataka**  >  **Policy**.
3. Odredite pravila koja se odnose na web-mjesta sustava SharePoint i izmijenite pravilo tako da web-mjesto sustava SharePoint za tim koji sadrži privatni kanal nije obuhvaćeno Pravilnikom o zadržavanju.
4. Spremanje pravilnika.
    Postavke pravilnika mogu potrajati i do 24 sata.
    Kada je web-mjesto isključeno, možete izbrisati privatni kanal.  
    
***Možda*** ćete moći izbrisati privatni kanal pomoću Microsoftovih timova na uređaju sa sustavom Android. 

Za srodne informacije sustava SharePoint pročitajte članak [nije moguće izbrisati stavke u sustavu SharePoint Online ni na servisu OneDrive za tvrtke](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).