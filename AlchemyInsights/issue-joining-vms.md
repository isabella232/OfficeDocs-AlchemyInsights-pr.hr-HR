---
title: Problem s pridruživanjem VMs-a
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884860"
---
# <a name="issue-joining-vms"></a>Problem s pridruživanjem VMs-a

Da biste riješili probleme koji se javljaju prilikom pokušaja pridruživanja VMs-u, slijedite sljedeće korake:

1. Pokušajte se prijaviti pomoću oblika **UPN** (primjerice, "joeuser@contoso.com") umjesto oblika **SAMAccountName** ("CONTOSO\joeuser").
2. Provjerite jeste li omogućili sinkronizaciju lozinki u skladu sa koracima navedenim u vodiču za *početak rada* .
3. Pobrinite se da izvještačen korisnički račun nije vanjski račun u zakupcu Azure AD. Vanjski se korisnici ne mogu prijaviti u upravljane domene budući da usluge Azure AD domena nemaju vjerodajnice za takve korisničke račune.
4. Ako je izvještačen korisnički račun korisnički račun samo u oblaku, provjerite jesu li korisnici promijenili lozinku nakon što ste omogućili usluge Azure AD domene. U ovom se koraku uzrokuje generiranje skice vjerodajnica potrebnih za izvoz servisa Azure AD Domain.
5. Ako se prijavljeni korisnički računi sinkroniziraju iz lokalnog direktorija, provjerite je li preporučeno izdanje servisa Azure AD Connect konfigurirano za kompletnu sinkronizaciju.
6. Ako se problem nastavi pojavljivati i nakon potvrđene četvrtog koraka, izvršite sljedeće naredbe na uređaju za sinkronizaciju:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.