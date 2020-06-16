---
title: Otklanjanje poteškoća sa servisom OneDrive ruši se
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748797"
---
# <a name="troubleshoot-onedrive-crashes"></a>Otklanjanje poteškoća sa servisom OneDrive ruši se

Ako se OneDrive više puta ruši, isprobajte sljedeće korake za otklanjanje poteškoća:

**Provjerite nisu li ključevi registra postavljeni:**

1. Pomoću uređivača registra idite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ako je DisableFileSyncNGSC prisutan i postavljen na 1, otvorite tipku i promijenite vrijednost na 0.
3. Ručno pokretanje servisa OneDrive tako da otvorite Start ![Pritisnite tipku Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.

**Vraćanje izvornih postavki servisa OneDrive:**

Bilješke:

- Vraćanjem na servis OneDrive prekidaju se sve postojeće sinkronizacijske veze (uključujući osobni servis OneDrive ako je postavljen).
- Nećete izgubiti datoteke ili podatke tako da ponovno postavite OneDrive na računalu.

**Da biste vratili izvorne postavke servisa OneDrive:**

1. Otvorite dijaloški okvir Pokreni pritiskom na tipku Sustava Windows i R.
2. Upišite %localappdata%\Microsoft\OneDrive\onedrive.exe /resetiraj i pritisnite OK. Može se nakratko pojaviti prozor naredbe.
3. Ručno pokretanje servisa OneDrive tako da otvorite Start ![Pritisnite tipku Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.

Bilješke:

- Ako ste odabrali sinkronizaciju samo nekih mapa prije ponovnog postavljanja, morat ćete to učiniti ponovno nakon dovršetka sinkronizacije. Dodatne informacije [potražite u odjeljku Odaberite mape servisa OneDrive za sinkronizaciju s računalom.](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)  
- To ćete morati dovršiti za osobne OneDrive i OneDrive za tvrtke.