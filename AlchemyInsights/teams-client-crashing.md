---
title: Teams klijent se ruši
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: bef16351b55ac4765539d66ab86a71183f66f0dd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321617"
---
# <a name="teams-client-crashing"></a>Teams klijent se ruši

Ako vam se klijent za Teams ruši, pokušajte sljedeće:

- Ako koristite Teams za stolna računala, [provjerite je li program u potpunosti ažuriran](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Provjerite jesu li [dostupni Microsoft 365 URL-ovi](https://docs.microsoft.com/microsoftteams/connectivity-issues) i rasponi adresa.

- Prijavite se pomoću administratorskog računa klijenta i provjerite nadzornu ploču [stanja](https://docs.microsoft.com/office365/enterprise/view-service-health) servisa da biste provjerili ne postoji li nedostatak ili degradacija servisa.

- Deinstalacija i ponovna instalacija Teams aplikacije
    - Pronađite mapu %appdata%\Microsoft\Teams\ na računalu i izbrišite sve datoteke u tom direktoriju.
    - [Preuzmite i instalirajte aplikaciju Teams ,](https://www.microsoft.com/microsoft-teams/download-app)a ako je moguće, instalirajte Teams kao administrator (desnom tipkom miša kliknite instalacijski program Teams pa odaberite **Pokreni kao administrator** ako je dostupan).

Ako se Teams i dalje ruši, pokušajte reproducirati problem. Ako možete:

1. Pomoću snimača koraka snimite korake.
    - Zatvorite sve nepotrebne ili povjerljive aplikacije.
    - Pokrenite snimač koraka i reproducirajte problem dok ste prijavljeni s zahvaćenim korisničkim računom.
    - [Prikupite zapisnike timova koji snimaju snimljene korake za reprodukciju](https://docs.microsoft.com/microsoftteams/log-files). 
    
    **Napomena**: provjerite jeste li snimili adresu za prijavu na koju je korisnik na to utječe.
    - Prikupite podatke o izvatkom i/ili košu kvara (Windows). Pokrenite Windows powershell na uređaju na kojem se ruši i pokrenite sljedeće naredbe (nakon svake naredbe pritisnite Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Kada se tekstna datoteka generira i prikaže na zaslonu, spremite datoteku i priložite je zahtjevu za servis. 
