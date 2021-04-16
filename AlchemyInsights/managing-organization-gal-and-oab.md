---
title: Upravljanje globalnim popisom adresa tvrtke ili ustanove i izvanmrežnim adresarom
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794824"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>Upravljanje globalnim popisom adresa tvrtke ili ustanove (GAL) i izvanmrežnim adresarom (OAB)

Globalni popis adresa (GAL) popis je objekata s omogućenom e-poštom (svih vrsta primatelja koji mogu primati e-poštu) u tvrtki ili ustanovi. Jedan se GAL automatski stvara u svakoj tvrtki ili ustanovi. Možete stvarati dodatne GAL-ove da biste razdvojili korisnike po tvrtki ili ustanovi ili mjestu, ali jedan korisnik može istodobno vidjeti i koristiti samo jedan GAL.

Neki klijenti za e-poštu, kao što je Outlook za Windows, preuzimaju GAL za izvanmrežni rad. To je poznato kao izvanmrežni adresar (OAB). U sustavu Exchange online OAB se ažurira samo jedanput svakih 8 sati, a potom ga klijenti moraju preuzeti da bi ažurirali svoju lokalnu kopiju OAB-a. Svaka promjena primatelja mora najprije biti vidljiva u GAL-u da bi se kasnije mogla prenijeti u OAB.

Evo nekoliko uobičajenih postupaka koji se koriste za GAL i OAB:

- Zbog niza razloga dobro je sakriti neke objekte od GAL-a. Pročitajte članak [Sakrivanje primatelja od popisa adresa](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).
- Ako trebate pojedinim grupama korisnika omogućiti prilagođene prikaze GAL-a tvrtke ili ustanove, pročitajte članak [Pravilnici za adresare u sustavu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- [Stvorite globalni popis adresa u sustavu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list), a da biste saznali kako raditi s dozvolama za GAL, pročitajte članak [Popisi adresa u sustavu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists). Imajte na umu da je, ako stvarate nove GAL-ove, dobro stvoriti i novi OAB. Pročitajte članak [Postupci s izvanmrežnim adresarom](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).
