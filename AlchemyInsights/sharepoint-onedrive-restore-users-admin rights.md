---
title: Otklanjanje poteškoća s porukama odbijeno za web-mjesta OneDrive za tvrtke
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766703"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Otklanjanje poteškoća s porukama odbijeno za web-mjesta OneDrive za tvrtke

Taj se problem najčešće pojavljuje kada se korisnik izbriše i ponovno stvori s istim korisničkim nazivom (UPN). Novi račun kreira se pomoću različite vrijednosti PUID Kada korisnik pokuša pristupiti zbirci web-mjesta ili svom servisu OneDrive, korisnik ima neispravan PUID. Drugi scenarij uključuje sinkronizaciju direktorija s organizacijskom jedinicom Active Directory (OU). Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, možda će doživjeti taj problem.

1. Da biste riješili taj problem, trebali biste vratiti izvorni UPN s koracima u članku, [vratiti korisnika u Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Ako ne možete vratiti izvornog korisnika, morate ukloniti starog korisnika s web-mjesta OneDrive pomoću ovih koraka, [ukloniti korisnika s popisa korisničkih informacija](). 
3. Nakon što je to učinjeno, možete provjeriti korisnik ima administratorska prava na OneDrive web-mjesta slijedeći korake za [Dodavanje admin-a za user ' s OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Dodatne informacije o razinama dozvola potražite u članku, [razumijevanje razina dozvola u sustavu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
