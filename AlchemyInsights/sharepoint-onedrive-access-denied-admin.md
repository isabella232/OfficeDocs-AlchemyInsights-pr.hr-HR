---
title: Otklanjanje poteškoća s porukama koje su odbijene pristupom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505371"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Otklanjanje poteškoća s porukama o pristupu u centru za administratore sustava SharePoint/OneDrive

Ako prilikom pokušaja pregledavanja centra za administratore sustava SharePoint/OneDrive primate poruku o odbijenom pristupu, provjerite jeste li [korisniku dodijelili licencu](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Ako korisnik ima licencu, provjerite je li [im dodijeljena administratorska uloga](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) koja može pristupiti centrima za administratore.

Taj se problem može pojaviti i kada se korisnik izbriše i ponovno stvori s istim glavnim nazivom korisnika (UPN). Novi račun stvara se pomoću druge vrijednosti PUID (Passport Unique ID). Kada korisnik pokuša pristupiti zbirci web-mjesta ili na servisu OneDrive, korisnik ima neispravan PUID. Drugi scenarij uključuje sinkronizaciju direktorija s organizacijskom jedinicom servisa Active Directory (OU). Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, možda će naići na taj problem.

Da biste riješili taj problem, trebali biste vratiti izvorni UPN s koracima u članku [Vraćanje korisnika u sustavu Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Napomena: ako centar za administratore servisa OneDrive ili SharePoint nije dostupan većem broju korisnika koji su prethodno imali pristup, možda postoji problem s privremenim servisom.  [Provjerite nadzornu ploču stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).


