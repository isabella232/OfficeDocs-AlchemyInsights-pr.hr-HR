---
title: Problemi performanse-SharePoint ili OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 9bb18196f38de473e4ee79d77bd43561ad9742e0
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223272"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ili OneDrive spora, nedostupni ili nedostupna za više korisnika

Ako OneDrive ili SharePoint web-mjesta nije dostupno više korisnike koji su prethodno imali pristup, možda postoji problem privremeni servisa. [Provjerite servisa stanja nadzorne ploče](https://portal.office.com/adminportal/home#/servicehealth).

**Dodajte i licence korisnika**

Provjerite koje ste [dodijelili licence korisnicima u Office 365 poslovne](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


**Dodijelite dozvole**

Ako korisnik je dodijeljena licenca Sharepoint i još uvijek primanje uskraćen pristup, provjerite je li imati [odgovarajuću razinu dozvole](https://docs.microsoft.com/sharepoint/understanding-permission-levels) dodijeljene.

**Razmislite o korištenju značajke zahtjeva pristupa**

[Značajka zahtjev access](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućuje korisnicima zatražili pristup sadržaju trenutno nemaju dozvolu za prikaz.

**Dopusti Prilagođena skripta može uzrokovati pristup odbijen problemi**

Postoje određene scenarije gdje značajka *Dopusti prilagođene skripte* možda biti dosljedna odbijen pristup. Za popis utječe na sljedeće značajke, Sigurnosna razmatranja i onemogućiti značajku. Posjetite [Dopusti ili spriječiti prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

