---
title: Apple MDM push certifikat nije postavljen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438853"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM push certifikat nije postavljen

AppleM push certifikat (poznat i kao certifikat servisa za slanje push obavijesti tvrtke Apple) nije konfiguriran za vašu pretplatu. Bez konfiguriranog Apple MDM push certifikata ne možete prijaviti i upravljati uređajima sa sustavom iOS i Mac OS. Nakon što dodate certifikat u Intune, korisnici mogu instalirati aplikaciju Portal tvrtke da bi prijavili svoje iOS uređaje.

1. Odaberite **"Slažem se".** da biste Microsoftu dali dozvolu za slanje podataka Appleu.

2. Odaberite **Preuzmite CSR** zahtjev za potpisivanje intune certifikata potreban za izradu Apple MDM push certifikata. Datoteka se koristi za traženje certifikata pouzdanog odnosa s Appleovog portala push certifikata.

3. Odaberite **Izradi MDM push certifikat** da biste otišli na Apple push certificates portal. Prijavite se pomoću Apple ID-a tvrtke, a zatim odaberite **Stvori certifikat**. Odaberite **Odaberi datoteku**, pronađite datoteku zahtjeva za potpisivanje certifikata, a zatim odaberite **Prijenos**. Na stranici Potvrda odaberite **Preuzmi** da biste preuzeli datoteku certifikata (.pem) i spremite datoteku lokalno.
 
**Napomena:** Certifikat je povezan s Apple ID-om koji se koristi za stvaranje. Kao najbolju praksu koristite tvrtku Apple ID za zadatke upravljanja i provjerite nadzire li poštanski sandučić više osoba ili pomoću popisa za distribuciju. Nikada ne koristite osobni Apple ID. Koristite isti Apple ID za obnovu Apple push certifikata svakih 12 mjeseci.
 
4. Unesite Apple ID koji se koristi za izradu Apple MDM push certifikata. Zabilježite ovaj ID kao podsjetnik kada trebate obnoviti certifikat.

5. Idite na datoteku certifikata (.pem), odaberite **Otvori**, a zatim **prenesi**. Pomoću push certifikata Intune može upisati Apple uređaje i upravljati njima.