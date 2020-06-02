---
title: Problemi s performansama- SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511140"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>Spor, nedostupan ili nedostupan za više korisnika sustava SharePoint ili OneDrive

Ako web-mjesto servisa OneDrive ili SharePoint nije dostupno većem broju korisnika koji su prethodno imali pristup, možda postoji problem s privremenim servisom. [Provjerite nadzornu ploču stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).

**Dodavanje i licenciranje korisnika**

Provjerite dodijelite li [licence korisnicima u sustavu Microsoft 365 za tvrtke](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Dodijeli dozvole**

Ako je korisniku dodijeljena licenca za Sharepoint i još uvijek prima poruku odbijenog pristupa, provjerite je li dodijeljena [odgovarajuća razina dozvole.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**Razmislite o korištenju značajke zahtjeva za pristup**

[Značajka zahtjeva za pristup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućuje korisnicima da zatraže pristup sadržaju za koji trenutno nemaju dozvolu za prikaz.

**Dopusti prilagođenu skriptu može uzrokovati probleme s odbijenim pristupom**

Postoje određeni scenariji u kojima značajka *Dopusti prilagođenu skriptu* možda predstavlja pristup odbijen. Za popis značajki na koje se to odnosi, sigurnosna razmatranja i mogućnost onemogućivanja značajke. Posjetite [Dopusti ili spriječite prilagođenu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

