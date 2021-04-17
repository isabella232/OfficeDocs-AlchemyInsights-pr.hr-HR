---
title: Otklanjanje poteškoća sa servisom OneDrive
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
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826191"
---
# <a name="troubleshoot-onedrive-crashes"></a>Otklanjanje poteškoća sa servisom OneDrive

Ako se OneDrive više puta ruši, isprobajte sljedeće korake za otklanjanje poteškoća:

**Provjerite nisu li ključevi registra postavljeni:**

1. Pomoću uređivača registra idite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ako je disableFileSyncNGSC prisutan i postavljen na 1, otvorite ključ i promijenite vrijednost u 0.
3. Ručno pokretanje servisa OneDrive na izborniku Start ![Pritiskanje tipke sustava Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.

**Ponovno postavljanje servisa OneDrive:**

Napomene:

- Ponovno postavljanje servisa OneDrive prekida vezu sa svim postojećim vezama za sinkronizaciju (uključujući osobni OneDrive ako je postavljen).
- Nećete izgubiti datoteke ni podatke tako da ponovno na računalu ponovno e-postavljanjem servisa OneDrive.

**Ponovno postavljanje servisa OneDrive:**

1. Otvorite dijaloški okvir Pokreni pritiskom na tipku Windows i R.
2. Upišite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset pa pritisnite U redu. Nakratko se može pojaviti prozor Naredbe.
3. Ručno pokretanje servisa OneDrive na izborniku Start ![Pritiskanje tipke sustava Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.

Napomene:

- Ako ste prije vraćanja na izvorno odabrali sinkronizaciju samo nekih mapa, morat ćete to ponoviti kada se sinkronizacija dovrši. Dodatne [informacije potražite u odabiru mapa servisa OneDrive koje](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)želite   sinkronizirati s računalom.
- To ćete morati dovršiti za osobni OneDrive i OneDrive za tvrtke.