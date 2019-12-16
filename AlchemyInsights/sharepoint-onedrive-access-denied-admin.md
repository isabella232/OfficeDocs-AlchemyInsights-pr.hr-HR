---
title: Otklanjanje poteškoća s porukama odbijeno za pristup
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051417"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Otklanjanje poteškoća s porukama odbijeno u centru za administraciju sustava SharePoint/OneDrive

Ako primite poruku o odbijanju pristupa prilikom pokušaja pregledavanja u centar za administraciju sustava SharePoint/OneDrive, provjerite jeste li [korisniku dodijelili licencu](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Ako korisnik ima licencu, također biste trebali osigurati da im je [dodijeljena administratorska uloga](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) koja može pristupiti centrima za administraciju.

Taj se problem može pojaviti i kada se korisnik izbriše i ponovno stvori s istim korisničkim nazivom (UPN). Novi račun kreira se pomoću različite vrijednosti PUID Kada korisnik pokuša pristupiti zbirci web-mjesta ili svom servisu OneDrive, korisnik ima neispravan PUID. Drugi scenarij uključuje sinkronizaciju direktorija s organizacijskom jedinicom Active Directory (OU). Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, možda će doživjeti taj problem.

Da biste riješili taj problem, trebali biste vratiti izvorni UPN s koracima u članku, [vratiti korisnika u Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Napomena: Ako servis OneDrive ili SharePoint admin centar nije dostupan više korisnika koji su ranije imali pristup, možda postoji problem privremenog servisa.  [Provjerite nadzornu ploču zdravstvenog stanja usluge](https://portal.office.com/adminportal/home#/servicehealth).


