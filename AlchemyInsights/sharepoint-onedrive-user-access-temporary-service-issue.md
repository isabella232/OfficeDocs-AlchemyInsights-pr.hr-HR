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
ms.openlocfilehash: 880b2bdd7b74f4365bcbff73a709d42e72be0e3a
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36535147"
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

