---
title: AppleOV MDM push certificate nije postavljen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 4f8e3502a7be35b5579ec1436852fe2bff9b1316891c7a9020f6f5f4767b3d88
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931519"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>AppleOV MDM push certificate nije postavljen

Appleov MDM push certificate (poznat i kao Appleov certifikat servisa za slanje obavijesti (APNS) nije konfiguriran za vašu pretplatu. Bez konfiguriranog appleova MDM push certifikata ne možete se prijaviti i upravljati uređajima sa sustavom iOS i Mac OS. Kada certifikat dodate u Intune, korisnici mogu instalirati aplikaciju Company Portal za registraciju uređaja sa sustavom iOS.

1. Odaberite **"Slažem se".** da biste Microsoftu dali dozvolu za slanje podataka Appleu.

2. Odaberite **Preuzmi CSR** zahtjev za potpisivanje certifikata Intune koji je potreban za stvaranje appleova MDM push certifikata. Datoteka se koristi za zahtjev za certifikat odnosa pouzdanosti s Appleova portala za push certifikate.

3. Odaberite **Stvori MDM push certificate da biste** se idite na Appleov portal za push certifikate. Prijavite se pomoću Apple ID-a tvrtke, a zatim **odaberite Stvori certifikat**. Odaberite **Odaberite Datoteka**, dođite do datoteke zahtjeva za potpisivanje certifikata, a zatim **odaberite Prijenos**. Na stranici Potvrda odaberite **Preuzmi** da biste preuzeli datoteku certifikata (.pem) pa spremite datoteku lokalno.
 
**Napomena:** certifikat je povezan s Apple ID-om koji se koristi za stvaranje certifikata. Kao najbolje prakse koristite Apple ID tvrtke za zadatke upravljanja i provjerite nadzire li poštanski sandučić više osoba ili pomoću popisa za raspodjelu. Nikad nemojte koristiti osobni Apple ID. Isti Apple ID koristite za obnovu Appleova push certifikata svakih 12 mjeseci.
 
4. Unesite Apple ID koji se koristi za stvaranje Apple MDM push certifikata. Zabilježite taj ID kao podsjetnik kada morate obnoviti certifikat.

5. Idite na datoteku certifikata (.pem), **odaberite Otvori**, a zatim **odaberite Prijenos**. Uz push certifikat Intune može registrirati Appleove uređaje i upravljati njima.