---
title: Problemi s performansama – SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771236"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ili OneDrive spori, nedostupni ili nedostupni za više korisnika

Ako web-mjesto servisa OneDrive ili SharePoint nije dostupno većem broju korisnika koji su prethodno imali pristup, možda postoji privremeni problem s servisom. [Provjerite nadzornu ploču zdravstvenog stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).

**Dodavanje i licenciranje korisnika**

Provjerite jeste li [korisnicima dodijelili licence u programu Microsoft 365 za tvrtke](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Dodjela dozvola**

Ako je korisniku dodijeljena licenca za SharePoint i još uvijek dobiva poruku o uskraćenom pristupu, provjerite ima li dodijeljenu [odgovarajuću razinu dozvola](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**Razmislite o korištenju značajke zahtjeva za Access**

[Značajka zahtjeva za pristup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućuje korisnicima da zatraže pristup sadržaju koji trenutno nemaju dozvolu za pregled.

**Omogućivanje prilagođene skripte može uzrokovati probleme s uskraćanjem programa Access**

Postoje određeni scenariji u kojima značajka *Dopusti prilagođenu skriptu* može prikazati zabranjen pristup. Popis značajki koje su zahvaćene sigurnosnim razmišljanjima i mogućnost onemogućivanja značajke. Posjetite [Dopusti ili spriječi prilagođenu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

