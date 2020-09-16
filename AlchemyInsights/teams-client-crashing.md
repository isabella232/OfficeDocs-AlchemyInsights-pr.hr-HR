---
title: Klijent za Teams se ruši?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691099"
---
# <a name="teams-client-crashing"></a>Klijent za Teams se ruši?

Ako vam se klijent za Teams ruši, pokušajte sljedeće:

- Ako koristite Teams za stolna računala, [provjerite je li program u potpunosti ažuriran](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Provjerite jesu li svi [URL-ovi i rasponi microsoftova 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) dostupni.

- Prijavite se pomoću računa za administratore korisnika i provjerite postoji li [kontrolna tabla zdravstvenog stanja](https://docs.microsoft.com/office365/enterprise/view-service-health) da biste provjerili postoji li propadanje ili degradacija servisa.

- Deinstalacija i ponovna instalacija aplikacije timovi (veza)
    - Dođite do% AppData%\microsoft\teams\ folder na računalu i izbrišite sve datoteke u tom direktoriju.
    - [Preuzmite i instalirajte aplikaciju timovi](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), a ako je moguće, instalirajte timove kao administratore (desnom tipkom miša kliknite instalacijski program za timove, a zatim odaberite "Pokreni kao administrator" Ako je dostupno).

Ako vam se klijent za timove i dalje ruši, možete li ponoviti problem? Ako je tako, učinite sljedeće:

1. Upotrijebite snimač koraka da biste snimili korake.
    - Zatvaranje svih nepotrebnih ili povjerljivih aplikacija.
    - Pokrenite snimač koraka i reproducirajte problem dok ste prijavljeni uz izvještačen korisnički račun.
    - [Prikupite zapisnike timova koji snimaju snimljene reproducirajte korake](https://docs.microsoft.com/microsoftteams/log-files). **Pažnja**: Provjerite jeste li snimili adresu za prijavu na korisnika koji je utjecao na njega.
    - Prikupljanje podataka o izvatkom i/ili kvaru (Windows). Pokrenite Windows PowerShell na stroju na kojem se pojavljuje sudar i pokrenite sljedeće naredbe:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Priložite datoteku u slučaj podrške.
