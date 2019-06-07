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
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760333"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Pristup odbijen poruke u centru Sharepoint OneDrive Admin rješavanje problema

Ako primate uskraćen prilikom pokušaja Pregledaj centar Admin Sharepoint OneDrive pristup, provjerite je li taj [dodeljivanje licence korisniku](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Ako korisnik ima licencu, također provjerite su [dodijeljeni ulogu administratora](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) koji može pristupiti admin centre.

Ovaj se problem može pojaviti kada korisnik izbrisana i stvorena ponovo s istom korisniku glavni naziv (UPN). Novi račun stvorena pomoću različite PUID (jedinstveni ID Passport) vrijednost. Kada korisnik pokuša pristupiti zbirci web-mjesta ili njihovim OneDrive, korisnik ima neispravan PUID. Drugi scenarij uključuje imenik sinkronizacije s u Active Directory organizacijsku jedinicu (OU). Ako korisnici imaju već prijavljeni u SharePoint, a zatim su premještene različite OU i resynced SharePoint, može doći taj problem.

Da biste riješili taj problem, trebali biste vratiti izvornu UPN s korake u članku [Vraćanje korisnika u Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Napomena: Ako centar za OneDrive ili SharePoint administraciju nije dostupno više korisnike koji su prethodno imali pristup, možda postoji problem privremeni servisa.  [Provjerite servisa stanja nadzorne ploče](https://portal.office.com/adminportal/home#/servicehealth).


