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
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736640"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Daj korisnicima pristup SharePoint i OneDrive

Problem se najčešće pojavljuje kada korisnik izbrisana i stvorena ponovo s istom korisniku glavni naziv (UPN). Novi račun stvorena pomoću različite PUID (jedinstveni ID Passport) vrijednost. Kada korisnik pokuša pristupiti zbirci web-mjesta ili njihovim OneDrive, korisnik ima neispravan PUID. Drugi scenarij uključuje imenik sinkronizacije s u Active Directory organizacijsku jedinicu (OU). Ako korisnici imaju već prijavljeni u SharePoint, a zatim su premještene različite OU i resynced SharePoint, može doći taj problem.

Da biste riješili ovaj problem treba vratiti izvornu UPN s korake u članku[Vraćanje korisnika u Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).

Nakon što je napravljen, možete provjeriti korisnik ima prava administracije web-mjesta OneDrive slijedeći korake za [Dodavanje admin's za korisnika OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Dodatne informacije o razinama dozvola potražite u članku [Razumijevanje razine dozvola u programu SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).