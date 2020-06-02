---
title: Otklanjanje poteškoća s pristupom odbijene poruke na web-mjestima servisa OneDrive za tvrtke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511176"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Otklanjanje poteškoća s pristupom odbijene poruke na web-mjestima servisa OneDrive za tvrtke

Taj se problem najčešće pojavljuje kada se korisnik izbriše i ponovno stvori s istim glavnim nazivom korisnika (UPN). Novi račun stvara se pomoću druge vrijednosti PUID (Passport Unique ID). Kada korisnik pokuša pristupiti zbirci web-mjesta ili na servisu OneDrive, korisnik ima neispravan PUID. Drugi scenarij uključuje sinkronizaciju direktorija s organizacijskom jedinicom servisa Active Directory (OU). Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, možda će naići na taj problem.

1. Da biste riješili taj problem trebali biste vratiti izvorni UPN s koracima u [članku, Vraćanje korisnika u microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ako ne možete vratiti izvornog korisnika, trebali biste ukloniti starog korisnika s web-mjesta servisa OneDrive pomoću ovih [koraka, Uklonite korisnika s popisa korisničkih podataka](). 
3. Nakon što to učinite, možete provjeriti korisnik ima administratorska prava na web-mjesto servisa OneDrive slijedeći korake za [dodavanje administratora za korisnikov OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Dodatne informacije o razinama dozvola potražite u članku [Razumijevanje razina dozvola u sustavu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
