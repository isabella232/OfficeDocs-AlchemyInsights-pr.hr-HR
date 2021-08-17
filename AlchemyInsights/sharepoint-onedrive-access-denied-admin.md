---
title: Otklanjanje poteškoća s porukama koje su odbijene u programu Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085220"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Otklanjanje poteškoća s odbijenim porukama programa Access u sustavu Sharepoint/OneDrive centru za administratore

Ako prilikom pregledavanja centra za administratore sustava Sharepoint/OneDrive primate poruku o uskraćenom pristupu, provjerite jeste li korisniku [dodijelili licencu.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Ako korisnik ima licencu, morate se pobrinuti i da im se dodijeli [administratorska uloga koja](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) može pristupiti centrima za administratore.

Taj se problem može pojaviti i kada se korisnik izbriše i ponovno stvori s istim korisničkim glavnim imenom (UPN- om). Novi se račun stvara pomoću druge vrijednosti PUID (Passport Unique ID). Kada korisnik pokuša pristupiti zbirci web-mjesta ili OneDrive, korisnik ima netočan PUID. Drugi scenarij obuhvaća sinkronizaciju direktorija s organizacijskom jedinicom servisa Active Directory (OU). Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju s SharePoint, možda će naići na taj problem.

Da biste riješili taj problem, trebali biste vratiti izvorni UPN pomoću koraka u članku Vraćanje [korisnika u programu Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Napomena: ako centar OneDrive ili SharePoint nije dostupan više korisnika koji su prethodno imali pristup, možda postoji privremeni problem sa servisom.  [Provjerite nadzornu ploču stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).


