---
title: Otklanjanje poteškoća s prekidima servisa OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664990"
---
# <a name="troubleshoot-onedrive-crashes"></a>Otklanjanje poteškoća s prekidima servisa OneDrive

Ako se OneDrive opetovano ruši, isprobajte ove korake za otklanjanje poteškoća:

**Provjerite nisu li postavljeni ključevi registra:**

1. Pomoću uređivača registra dođite do HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Ako je prisutan DisableFileSyncNGSC i postavljen na 1, otvorite ključ i promijenite vrijednost u 0.
3. Ručno pokretanje servisa OneDrive tako da počnete s pokretanjem ![Pritišćite tipku sa sustavom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.

**Ponovno postavljanje servisa OneDrive:**

Bilješke

- Ponovnim postavljanjem servisa OneDrive prekida se sve postojeće Sinkronizacijske veze (uključujući osobni OneDrive ako je postavljeno).
- Datoteke i podatke nećete izgubiti ponovnim postavljanjem servisa OneDrive na računalu.

**Da biste ponovno postavili OneDrive:**

1. Otvorite dijaloški okvir Pokreni tako da pritisnete tipku sustava Windows i R.
2. Upišite% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset i pritisnite u redu. Naredbeni se prozor može pojaviti kratko.
3. Ručno pokretanje servisa OneDrive tako da počnete s pokretanjem ![Pritišćite tipku sa sustavom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.

Bilješke

- Ako ste odabrali sinkronizaciju samo nekih mapa prije ponovnog postavljanja, morat ćete to učiniti ponovno nakon dovršetka sinkronizacije. Dodatne informacije potražite u odjeljku [Odabir mapa servisa OneDrive za sinkronizaciju s računalom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .
- To ćete morati dovršiti radi osobnog servisa OneDrive i servisa OneDrive za tvrtke.