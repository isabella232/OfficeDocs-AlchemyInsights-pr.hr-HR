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
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719509"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ili OneDrive spora, nedostupni ili nedostupna za više korisnika

Ako OneDrive ili SharePoint web-mjesta nije dostupno više korisnike koji su prethodno imali pristup, možda postoji problem privremeni servisa. [Provjerite servisa stanja nadzorne ploče](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Dodajte i licence korisnika

Provjerite koje ste [dodijelili licence korisnicima u Office 365 poslovne](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Dodijelite dozvole

Ako korisnik je dodijeljena licenca Sharepoint i još uvijek primanje uskraćen pristup, provjerite je li imati [odgovarajuću razinu dozvole](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) dodijeljene.

## <a name="consider-using-the-access-request-feature"></a>Razmislite o korištenju značajke zahtjeva pristupa

[Značajka zahtjev access](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućuje korisnicima zatražili pristup sadržaju trenutno nemaju dozvolu za prikaz.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Dopusti Prilagođena skripta može uzrokovati pristup odbijen problemi

Postoje određene scenarije gdje značajka *Dopusti prilagođene skripte* možda biti dosljedna odbijen pristup. Za popis utječe na sljedeće značajke, Sigurnosna razmatranja i onemogućiti značajku. Posjetite [Dopusti ili spriječiti prilagođene skripte](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

