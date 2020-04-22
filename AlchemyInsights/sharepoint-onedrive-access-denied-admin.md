---
title: Otklanjanje poteškoća s porukama odbijenim pristupom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758377"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Otklanjanje poteškoća s porukama u kojima je odbijen pristup u centru za administratore sustava Sharepoint/OneDrive

Ako prilikom pokušaja pregleda u centru za administratore sustava Sharepoint/OneDrive primite poruku odbijenog pristupa, svakako [dodijelite licencu korisniku](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Ako korisnik ima licencu, provjerite im [dodijeljenu administratorsku ulogu](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) koja može pristupiti centrima za administratore.

Taj se problem može pojaviti i kada se korisnik izbriše i ponovno stvori s istim korisničkim glavnim nazivom (UPN). Novi račun stvara se pomoću različite VRIJEDNOSTI PUID (Passport Unique ID). Kada korisnik pokuša pristupiti zbirci web-mjesta ili na servisu OneDrive, korisnik ima pogrešan PUID. Drugi scenarij uključuje sinkronizaciju direktorija s organizacijskom jedinicom servisa Active Directory (OU). Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, mogu se pojaviti taj problem.

Da biste riješili taj problem, trebali biste vratiti izvorni UPN s koracima iz članka, [Vraćanje korisnika u Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Napomena: ako centar za administratore servisa OneDrive ili Sustava SharePoint nije dostupan većem broju korisnika koji su prethodno imali pristup, možda postoji problem s privremenim servisom.  [Provjerite nadzornu ploču stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).


