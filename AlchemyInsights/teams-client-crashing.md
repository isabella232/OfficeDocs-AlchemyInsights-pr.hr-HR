---
title: Klijent za Teams se ruši?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354044"
---
# <a name="teams-client-crashing"></a>Klijent za Teams se ruši?

Ako vam se klijent za Teams ruši, pokušajte sljedeće:

- Ako koristite Teams za stolna računala, [provjerite je li program u potpunosti ažuriran](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Provjerite jesu li dostupni svi [URL-ovi i rasponi adresa sustava Microsoft 365.](https://docs.microsoft.com/microsoftteams/connectivity-issues)

- Prijavite se pomoću računa administratora klijenta i provjerite [nadzornu ploču stanja servisa](https://docs.microsoft.com/office365/enterprise/view-service-health) da biste provjerili da ne postoji prekid ili degradacija usluge.

- Deinstalacija i ponovna instalacija aplikacije Teams (veza)
    - Pronađite mapu %appdata%\Microsoft\teams\ na računalu i izbrišite sve datoteke u tom direktoriju.
    - [Preuzmite i instalirajte aplikaciju Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), a ako je moguće, instalirajte Teams kao administrator (desnom tipkom miša kliknite instalacijski program Teams i odaberite "Pokreni kao administrator" ako je dostupno).

Ako se klijent timova još uvijek ruši, možete li reproducirati problem? Ako je tako:

1. Pomoću snimača koraka snimite korake.
    - Zatvorite SVE nepotrebne ili povjerljive aplikacije.
    - Pokrenite snimač koraka i reproducirajte problem dok ste prijavljeni pomoću zahvaćenog korisničkog računa.
    - [Prikupite zapisnike timova koji bilježe snimljene repro korake](https://docs.microsoft.com/microsoftteams/log-files). **Napomena:** Provjerite jeste li snimili adresu za prijavu zahvaćenog korisnika.
    - Prikupite podatke o izvatku i/ili kanti kvara (Windows). Pokrenite Windows Powershell na računalu na kojem se pojavljuju pad sustava i pokrenite sljedeće naredbe:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Priložite datoteku kućištu za podršku.
