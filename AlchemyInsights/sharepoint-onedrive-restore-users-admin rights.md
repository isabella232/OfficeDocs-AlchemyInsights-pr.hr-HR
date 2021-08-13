---
title: Otklanjanje poteškoća s pristupom odbijenim porukama OneDrive za tvrtke web-mjestima
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957785"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Otklanjanje poteškoća s pristupom odbijenim porukama OneDrive za tvrtke web-mjestima

Taj se problem najčešće pojavljuje kada se korisnik izbriše i ponovno stvori s istim korisničkim glavnim imenom (UPN- om). Novi se račun stvara pomoću druge vrijednosti PUID (Passport Unique ID). Kada korisnik pokuša pristupiti zbirci web-mjesta ili OneDrive, korisnik ima netočan PUID. Drugi scenarij obuhvaća sinkronizaciju direktorija s organizacijskom jedinicom servisa Active Directory (OU). Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju s SharePoint, možda će naići na taj problem.

1. Da biste riješili taj problem, morate vratiti izvorni UPN pomoću koraka u članku Vraćanje [korisnika u programu Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ako ne možete vratiti izvornog korisnika, trebali biste starog korisnika ukloniti s OneDrive web-mjesta pomoću ovih koraka, [Uklonite korisnika s popisa korisničkih podataka](). 
3. Kada to učinite, možete provjeriti ima li korisnik administratorska prava na web-OneDrive web-mjesto tako da slijedite upute za dodavanje administratora za [korisnikov OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Dodatne informacije o razinama dozvola potražite u članku Objašnjenje [razina dozvola u programu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
