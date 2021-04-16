---
title: OneDrive za tvrtke Web OneDrive preusmjerava na Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799981"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Preusmjereno na Delve nakon klika na OneDrive

Pogledajte naš detaljni vodič [za otklanjanje poteškoća](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

Da bi riješio taj problem, administrator korisnicima mora dodijeliti pravo stvaranja web-mjesta Moja web-mjesta. To je zato što se stranica servisa OneDrive za tvrtke stvara na web-mjestima Moja web-mjesta.

Da biste dodijelili to pravo, slijedite ove korake:

1. U centru za administratore sustava SharePoint kliknite **korisnički profili**.

2. U **odjeljku** Osobe kliknite Upravljanje **korisničkim dozvolama**.

3. Dodajte korisnike kojima su potrebne dozvole za stvaranje web-mjesta Moja web-mjesta. Ta je postavka po zadanom postavljena na **Svi osim vanjskih korisnika**.

4. Kada dodate korisnika, korisnike ili grupu, provjerite je li odabran dodani korisnik,  korisnici ili grupa, pomaknite se do odjeljka s dozvolama, a zatim potvrdite okvir pokraj mogućnosti Stvaranje osobnog web-mjesta (obavezno za osobni prostor za pohranu, sažetke sadržaja vijesti **i praćeni sadržaj).**

5. Kliknite **U redu**, a zatim neka korisnik otvori stranicu servisa OneDrive da biste stvorili web-mjesto.
