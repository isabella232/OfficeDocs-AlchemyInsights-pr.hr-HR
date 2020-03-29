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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030539"
---
# <a name="teams-client-crashing"></a>Klijent za Teams se ruši?

Ako vam se klijent za Teams ruši, pokušajte sljedeće:

- Ako koristite Teams za stolna računala, [provjerite je li program u potpunosti ažuriran](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Provjerite jesu li dostupni svi [URL-ovi i rasponi adresa sustava Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues).

- Prijavite se pomoću administratorskog računa i na [nadzornoj ploči stanja servisa](https://docs.microsoft.com/office365/enterprise/view-service-health) provjerite da nema prekida ili degradacije servisa.

 - Kao zadnji korak možete pokušati očistiti predmemoriju klijenta za Teams:

    1.  Izađite iz klijenta za Microsoft Teams za računala. Možete desnom tipkom miša kliknuti **Teams** u području palete na programskoj traci te kliknuti **Zatvori** ili pokrenuti upravitelj zadataka i u potpunosti ubiti proces.

    2.  Otvorite Eksplorer za datoteke i upišite %appdata%\Microsoft\teams.

    3.  Kad otvorite taj direktorij, vidjet ćete neke od ovih mapa:

         - Iz mape **Application Cache** otvorite Cache i izbrišite sve datoteke na mjestu  predmemorije: %appdata%\Microsoft\teams\application cache\cache.

        - Iz mape **Blob_storage** izbrišite sve datoteke: %appdata%\Microsoft\teams\ blob_storage.

        - Iz mape **Cache** izbrišite sve datoteke: %appdata%\Microsoft\teams\Cache.

        - Iz mape **databases** izbrišite sve datoteke: %appdata%\Microsoft\teams\databases.

        - Iz mape **GPUCache** izbrišite sve datoteke: %appdata%\Microsoft\teams\GPUcache.

        - Iz mape **IndexedDB** izbrišite .db datoteku: %appdata%\Microsoft\teams\IndexedDB.

        - Iz mape **Local storage** izbrišite sve datoteke: %appdata%\Microsoft\teams\Local Storage.

        - Na kraju iz mape **tmp** izbrišite sve datoteke: %appdata%\Microsoft\teams\tmp.

    4. Ponovno pokrenite klijent za Teams.
