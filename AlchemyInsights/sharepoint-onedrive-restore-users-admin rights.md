---
title: Daj korisnicima pristup SharePoint i OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a689769dab24e12832ddc0937bc5ddc3d71dbee3
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759248"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Daj korisnicima pristup SharePoint i OneDrive

Problem se najčešće pojavljuje kada korisnik izbrisana i stvorena ponovo s istom korisniku glavni naziv (UPN). Novi račun stvorena pomoću različite PUID (jedinstveni ID Passport) vrijednost. Kada korisnik pokuša pristupiti zbirci web-mjesta ili njihovim OneDrive, korisnik ima neispravan PUID. Drugi scenarij uključuje imenik sinkronizacije s u Active Directory organizacijsku jedinicu (OU). Ako korisnici imaju već prijavljeni u SharePoint, a zatim su premještene različite OU i resynced SharePoint, može doći taj problem.

Da biste riješili ovaj problem treba vratiti izvornu UPN s korake u članku[Vraćanje korisnika u Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Nakon što je napravljen, možete provjeriti korisnik ima prava administracije web-mjesta OneDrive slijedeći korake za [Dodavanje admin's za korisnika OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Dodatne informacije o razinama dozvola potražite u članku [Razumijevanje razine dozvola u programu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
