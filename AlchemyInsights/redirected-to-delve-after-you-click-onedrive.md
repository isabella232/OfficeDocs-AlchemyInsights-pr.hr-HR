---
title: Preusmjeravanje servisa OneDrive za tvrtke web-OneDrive na delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776371"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Preusmjereno na delve nakon klika na OneDrive

Pogledajte detaljan [Vodič za otklanjanje poteškoća](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

Da biste riješili taj problem, administrator mora dodijeliti korisnicima pravo na stvaranje web-mjesta moje web-mjesta. To je zato što se na mojim web-mjestima stvara stranica servisa OneDrive za tvrtke.

Da biste to ispravno dodijelili, slijedite ove korake:

1. U centru za administratore sustava SharePoint kliknite **korisnički profili**.

2. U odjeljku **osobe** kliknite **Upravljanje korisničkim dozvolama**.

3. Dodajte korisnike kojima su potrebne dozvole za stvaranje web-mjesta moje web-mjesta. Ta je postavka po zadanom postavljena na **sve osim za vanjske korisnike**.

4. Kada dodate korisnika, korisnike ili grupu, provjerite je li odabran dodani korisnik, korisnici ili grupa, pomaknite se do odjeljka **dozvole** , a zatim potvrdite okvir pokraj **stvaranja osobnog web-mjesta (obavezno za osobno skladištenje, sažetak sadržaja vijesti i praćeni sadržaj)**.

5. Kliknite **u redu**, a zatim neka korisnik potraži na stranici servisa OneDrive da bi stvorio web-mjesto.
