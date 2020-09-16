---
title: Certifikat za guranje u aplikaciji Apple MDM nije postavljen
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
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716849"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Certifikat za guranje u aplikaciji Apple MDM nije postavljen

Potvrda dodatka Apple MDM (poznata i kao certifikat servisa Apple push notifikaciju (APN) nije konfigurirana za vašu pretplatu. Bez konfiguriranog certifikata za Apple MDM, ne možete upisati i upravljati uređajima sa sustavom iOS i Mac OS. Kada dodate certifikat u Intune, korisnici mogu instalirati aplikaciju Portal tvrtke da bi upisali svoje iOS uređaje.

1. Odaberite **"Slažem** se". Da biste Microsoftu dopustili poslati podatke u Apple.

2. Odaberite **Preuzmi CSR** da biste stvorili certifikat za potpisivanje Intune certifikatom koji je potreban za stvaranje dodatka Apple MDM. Datoteka se koristi za zahtjev za certifikatom o pouzdanosti iz portala Appleov gumb za izdavanje certifikata.

3. Odaberite **Stvaranje certifikata za MDM** da biste prešli na portal Apple push certifikata. Prijavite se pomoću tvrtke Apple ID, a zatim odaberite **Stvori certifikat**. Odaberite **Odaberi datoteku**, dođite do datoteke zahtjeva za potpisivanje certifikata, a zatim odaberite **Prenesi**. Na stranici za potvrdu odaberite **Preuzmi** da biste preuzeli datoteku certifikata (. Pem) i spremili datoteku lokalno.
 
**Pažnja**: certifikat je povezan s Appleovim ID-om koji se koristi za stvaranje. Kao najbolja praksa koristite tvrtke Apple ID za zadatke upravljanja i provjerite nadzire li poštanski sandučić više osoba ili pomoću popisa za raspodjelu. Nikad ne koristite osobni ID Apple. Koristite isti Apple ID da biste obnovili certifikat Apple push svakih 12 mjeseci.
 
4. Unesite Apple ID koji se koristi za stvaranje certifikata za slanje Apple MDM-a. Snimite ovaj ID kao podsjetnik kada morate obnoviti certifikat.

5. Idite na datoteku certifikata (. Pem), odaberite **Otvori**, a zatim odaberite **Prenesi**. Uz certifikat push, Intune može upisati i upravljati uređajima sa sustavom Apple.