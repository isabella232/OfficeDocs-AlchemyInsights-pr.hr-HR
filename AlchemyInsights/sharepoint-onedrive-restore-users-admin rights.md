---
title: Otklanjanje poteškoća s pristupom odbijenim porukama na web-mjestima servisa OneDrive za tvrtke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692793"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Otklanjanje poteškoća s pristupom odbijenim porukama na web-mjestima servisa OneDrive za tvrtke

Taj se problem najčešće pojavljuje kada se korisnik izbriše i ponovno stvori s istim korisničkim glavnim nazivom (UPN). Novi račun stvara se pomoću različite VRIJEDNOSTI PUID (Passport Unique ID). Kada korisnik pokuša pristupiti zbirci web-mjesta ili na servisu OneDrive, korisnik ima pogrešan PUID. Drugi scenarij uključuje sinkronizaciju direktorija s organizacijskom jedinicom servisa Active Directory (OU). Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, mogu se pojaviti taj problem.

1. Da biste riješili taj problem, trebali biste vratiti izvorni UPN s koracima iz članka, [Vraćanje korisnika u microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Ako ne možete vratiti izvornog korisnika, trebali biste ukloniti starog korisnika s web-mjesta servisa OneDrive pomoću ovih [koraka, uklonite korisnika s popisa korisničkih podataka](). 
3. Nakon toga možete provjeriti ima li korisnik administratorska prava na web-mjesto servisa OneDrive slijedeći korake za [dodavanje administratora za web-pogon servisa OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) korisnika

Dodatne informacije o razinama dozvola potražite u članku [Objašnjenje razina dozvola u sustavu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
