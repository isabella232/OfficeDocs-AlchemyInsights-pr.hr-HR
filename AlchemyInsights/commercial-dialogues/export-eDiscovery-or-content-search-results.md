---
title: Izvoz rezultata pretraživanja Iotkrivanja i sadržaja
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481281"
---
# <a name="export-ediscoverycontent-search-results"></a>Izvoz rezultata pretraživanja Iotkrivanja i sadržaja

Možda ćete morati izvoziti rezultate pretraživanja u PST datoteku (iz e-pošte) ili na izvorne dokumente sustava Office (sa web-mjesta sustava SharePoint i servisa OneDrive za tvrtke). Ako je tako, učinite sljedeće:

- Provjerite je li vašem računu dodijeljeno odgovarajuće dozvole za izvoz. Dodatne informacije potražite u članku [Dodjela dozvola za otkriće](https://go.microsoft.com/fwlink/?linkid=2102406).
- Provjerite je li računalo zadovoljilo sve [preduvjete](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin). Nisu podržani Svi preglednici, kao što je Chrome.
- Da biste izvezli iz pretraživanja sadržaja: a. Otvorite centar za [sigurnosnu &](https://protection.office.com/contentsearch) i kliknite **Pretraživanje**, a zatim odaberite **Pretraživanje sadržaja**. Na stranici **Pretraživanje sadržaja** odaberite spremljeno pretraživanje.
    b. U oknu s detaljima u odjeljku **Izvoz rezultata na računalo** odaberite **Započni izvoz**. Ako izvozite više od 100K poštanskih sandučića, morat ćete koristiti PowerShell da biste preuzeli rezultate izvoza. Dodatne informacije potražite u članku [Izvoz rezultata iz više od 100K poštanskih sandučića](https://go.microsoft.com/fwlink/?linkid=2143861).

Dodatne informacije potražite u članku [Izvoz rezultata pretraživanja sadržaja](https://go.microsoft.com/fwlink/?linkid=2102118).