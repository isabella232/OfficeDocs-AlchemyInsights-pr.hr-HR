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
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093680"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ili OneDrive, nedostupni ili nedostupni za više korisnika

Ako web-OneDrive ili SharePoint web-mjesto nije dostupno više korisnika koji su prethodno imali pristup, možda postoji privremeni problem sa servisom. [Provjerite nadzornu ploču stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).

**Dodavanje i licenciranje korisnika**

Provjerite dodjeljujete [li licence korisnicima u Microsoft 365 za tvrtke](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Dodjela dozvola**

Ako je korisniku dodijeljena licenca za SharePoint i i dalje prima poruku o uskraćenom pristupu, provjerite je li mu [dodijeljena odgovarajuća razina](https://docs.microsoft.com/sharepoint/understanding-permission-levels) dozvola.

**Razmislite o korištenju značajke zahtjeva za pristup**

Značajka [zahtjeva za pristup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) korisnicima omogućuje da zatra i pristup sadržaju za koji trenutno nemaju dozvolu za pristup.

**Dopusti prilagođenu skriptu može uzrokovati probleme s pristupom koji su odbijeni**

Postoje određeni scenariji u kojima značajka *Dopusti prilagođenu skriptu* može predstavljati pristup koji je odbijen. Popis zahvaćenih značajki, sigurnosna pitanja i mogućnost onemogućivanja značajke. Posjetite Dopusti [ili spriječite prilagođenu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

