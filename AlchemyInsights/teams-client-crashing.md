---
title: Klijent za Teams se ruši?
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
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826263"
---
# <a name="teams-client-crashing"></a>Klijent za Teams se ruši?

Ako vam se klijent za Teams ruši, pokušajte sljedeće:

- Ako koristite Teams za stolna računala, [provjerite je li program u potpunosti ažuriran](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Provjerite jesu li dostupni svi URL-ovi i rasponi adresa za [Microsoft 365.](https://docs.microsoft.com/microsoftteams/connectivity-issues)

- Prijavite se pomoću administratorskog računa klijenta i provjerite nadzornu ploču [stanja](https://docs.microsoft.com/office365/enterprise/view-service-health) servisa da biste provjerili ne postoji li nedostatak ili degradacija servisa.

- Deinstalacija i ponovna instalacija aplikacije Teams (veza)
    - Pronađite mapu %appdata%\Microsoft\teams\ na računalu i izbrišite sve datoteke u tom direktoriju.
    - [Preuzmite i instalirajte aplikaciju Teams,](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)a ako je moguće, instalirajte Teams kao administrator (desnom tipkom miša kliknite instalacijski program aplikacije Teams i odaberite "Pokreni kao administrator" ako je dostupno).

Ako se klijent za Teams i dalje ruši, možete li reproducirati problem? Ako je tako:

1. Pomoću snimača koraka snimite korake.
    - Zatvorite sve nepotrebne ili povjerljive aplikacije.
    - Pokrenite snimač koraka i reproducirajte problem dok ste prijavljeni s zahvaćenim korisničkim računom.
    - [Prikupite zapisnike timova koji snimaju snimljene korake za reprodukciju](https://docs.microsoft.com/microsoftteams/log-files). **Napomena**: provjerite jeste li snimili adresu za prijavu na koju je korisnik na to utječe.
    - Prikupite podatke o smetlišu i/ili košu kvara (Windows). Pokrenite Windows Powershell na računalu na kojem se ruši i pokrenite sljedeće naredbe:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Priložite datoteku na slučaj podrške.
