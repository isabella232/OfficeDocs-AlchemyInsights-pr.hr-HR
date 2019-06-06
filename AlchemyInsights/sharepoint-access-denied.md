---
title: Rješavanje problema s porukama pristup odbijen
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 5958ad06ca905f713b5f56aa5c536e95a485f01c
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735730"
---
# <a name="troubleshoot-access-denied-messages"></a>Rješavanje problema s porukama pristup odbijen

Ako primate uskraćen prilikom pokušaja Pregledaj web-mjesta Sharepoint Online pristup, Molim pogledajte u ispod članaka.

## <a name="add-and-license-the-user"></a>Dodajte i licence korisnika

Provjerite koje ste [dodijelili licence korisnicima u Office 365 poslovne](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).

Dodijelite dozvole

Ako korisnik je dodijeljena licenca Sharepoint i još uvijek primanje uskraćen pristup, provjerite imaju [odgovarajuću razinu dozvole dodijeljene](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).

Razmislite o korištenju značajke zahtjeva pristupa

Značajka [zahtjev access](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućuje korisnicima zatražili pristup sadržaju trenutno nemaju dozvolu za prikaz. 

Dopusti Prilagođena skripta može uzrokovati pristup odbijen problemi

Postoje određene scenarije gdje "Dopusti Prilagođena skripta" značajka možda biti dosljedna odbijen pristup. Za popis utječe na sljedeće značajke, Sigurnosna razmatranja i onemogućiti značajku. Posjetite, [Dopusti ili spriječiti prilagođene skripte](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)

Napomena: Ako OneDrive ili SharePoint web-mjesta nije dostupno više korisnike koji su prethodno imali pristup, možda postoji problem privremeni servisa. [Provjerite servisa stanja nadzorne ploče](https://portal.office.com/adminportal/home#/servicehealth).


  

