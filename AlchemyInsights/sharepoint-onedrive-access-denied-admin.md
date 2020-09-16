---
title: Otklanjanje poteškoća s zabranom pristupa porukama
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767649"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Otklanjanje poteškoća s zabranom pristupa porukama u centru za administratore sustava SharePoint/OneDrive

Ako prilikom pokušaja pregledavanja u centar za administratore sustava SharePoint/OneDrive primate poruku o uskraćenog pristupa, provjerite jeste li [korisniku dodijelili licencu](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Ako korisnik ima licencu, trebali biste se pobrinuti i da im je [dodijeljena administratorska uloga](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) koja može pristupati centrima za administratore.

Taj se problem može pojaviti i kada je korisnik izbrisan i ponovno stvoren pomoću istog glavnog naziva korisnika (UPN). Novi se račun stvara pomoću različite vrijednosti za PUID (jedinstveni ID putovnice). Kada korisnik pokuša pristupiti zbirci web-mjesta ili njihovom servisu OneDrive, korisnik ima pogrešan PUID. Drugi scenarij obuhvaća sinkronizaciju direktorija s organizacijom Active Directory (OU). Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, možda će doživjeti taj problem.

Da biste riješili taj problem, trebali biste vratiti originalni UPN pomoću koraka u članku, [vratiti korisnika u programu Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Pažnja: Ako centar za administratore servisa OneDrive ili SharePoint nije dostupan većem broju korisnika koji su prethodno imali pristup, možda postoji privremeni problem s servisom.  [Provjerite nadzornu ploču zdravstvenog stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).


