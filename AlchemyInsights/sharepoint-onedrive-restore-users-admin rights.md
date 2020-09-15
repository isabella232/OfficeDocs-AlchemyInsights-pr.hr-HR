---
title: Otklanjanje poteškoća s zabranom pristupa porukama web-mjesta servisa OneDrive za tvrtke
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
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670608"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Otklanjanje poteškoća s zabranom pristupa porukama web-mjesta servisa OneDrive za tvrtke

Taj se problem najčešće pojavljuje kada je korisnik izbrisan i ponovno stvoren pomoću istog glavnog naziva korisnika (UPN). Novi se račun stvara pomoću različite vrijednosti za PUID (jedinstveni ID putovnice). Kada korisnik pokuša pristupiti zbirci web-mjesta ili njihovom servisu OneDrive, korisnik ima pogrešan PUID. Drugi scenarij obuhvaća sinkronizaciju direktorija s organizacijom Active Directory (OU). Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, možda će doživjeti taj problem.

1. Da biste riješili taj problem, trebali biste vratiti originalni UPN pomoću koraka u članku, [vratiti korisnika u programu Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ako ne možete vratiti izvornog korisnika, trebali biste ukloniti starog korisnika s web-mjesta servisa OneDrive pomoću ovih koraka, [ukloniti korisnika s popisa korisnički info](). 
3. Kada je to gotovo, možete potvrditi da korisnik ima administratorska prava na web-mjesto servisa OneDrive prateći korake za [Dodavanje administratora za korisnički OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) .

Dodatne informacije o razinama dozvola potražite u članku [razumijevanje razina dozvola u sustavu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
