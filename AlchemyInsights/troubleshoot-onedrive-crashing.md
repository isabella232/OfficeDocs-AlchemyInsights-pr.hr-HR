---
title: Otklanjanje poteškoća OneDrive se ruši
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
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53920999"
---
# <a name="troubleshoot-onedrive-crashes"></a>Otklanjanje poteškoća OneDrive se ruši

Ako OneDrive više puta ruši, isprobajte sljedeće korake za otklanjanje poteškoća:

**Provjerite nisu li ključevi registra postavljeni:**

1. Pomoću uređivača registra idite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ako je disableFileSyncNGSC prisutan i postavljen na 1, otvorite ključ i promijenite vrijednost u 0.
3. Ručno pokretanje OneDrive pomoću gumba Start ![Pritisnite tipku Windows tipki](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), upišite OneDrive u okvir za pretraživanje, a zatim kliknite aplikaciju OneDrive za stolna računala.

**Ponovno OneDrive:**

Napomene:

- Ponovno postavljanje OneDrive prekida sve postojeće veze za sinkronizaciju (uključujući osobne OneDrive ako su postavljene).
- Datoteke i podatke nećete izgubiti tako da ih ponovno OneDrive na računalu.

**Da biste ponovno OneDrive:**

1. Otvorite dijaloški okvir Pokreni tako da pritisnete Windows tipku i R.
2. Upišite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset pa pritisnite U redu. Nakratko se može pojaviti prozor Naredbe.
3. Ručno pokretanje OneDrive pomoću gumba Start ![Pritisnite tipku Windows tipki](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), upišite OneDrive u okvir za pretraživanje, a zatim kliknite aplikaciju OneDrive za stolna računala.

Napomene:

- Ako ste prije vraćanja na izvorno odabrali sinkronizaciju samo nekih mapa, morat ćete to ponoviti kada se sinkronizacija dovrši. Dodatne [informacije potražite u OneDrive odaberite koje mape](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)želite sinkronizirati s   računalom.
- To ćete morati dovršiti za osobnu OneDrive i OneDrive za tvrtke.