---
title: Praćenje uvjetnog pristupa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708666"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Praćenje uvjetnog pristupa za Exchange

Korisnici usmjereni na uvjetni pristup primit će obavijest e-poštom ako ne zadovoljavaju preduvjete za pristup vaše tvrtke ili ustanove. Da biste riješili, preporučujemo vam jedno ili više sljedećih rješenja:

- Ako se pretpostavlja da je uređaj upisan, savjetujte korisniku da otvori aplikaciju Portal tvrtke i provjerite prikazuje li se na portalu tvrtke. Ako se to ne dogodi, korisnik bi trebao upisati uređaj.
- Na portalu Azure idite na Intune > usklađenosti uređaja. U odjeljku monitor kliknite usklađenost uređaja. Prikažite izvješće o usklađenosti uređaja da biste provjerili je li korisnikov uređaj označenog kao usklađen.
- Na portalu Azure idite na Intune > usklađenosti uređaja. U odjeljku Upravljanje kliknite pravila. Na popisu pravilnika o usklađenosti provjerite je li profil dodijeljen vašem korisničkom uređaju. Ako nijedan profil nije dodijeljen, zatim Intune neće moći potvrditi status usklađenosti uređaja.
- Uredite korisnički zadatak uvjetnog pristupa.

1. Na portalu Azure idite na umetanje   >  pravilnika o **uvjetnom pristupu**  >  .
2. Na popisu odaberite pravilo.
3. Kliknite Korisnici i grupe.
4. Da biste neku određenu politiku usmjerili na nekoga, dodajte ih na popis uvrštavanje. Da biste bili sigurni da je osoba izostavljena iz pravilnika, dodajte ih na popis za izuzimanje.

Korisne veze:

[Pregled usklađenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)

[Otklanjanje poteškoća sa com](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Pravilnik o otklanjanju poteškoća](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Praćenje usklađivanja uređaja](https://docs.microsoft.com/intune/compliance-policy-monitor)

Pažnja: ovi su koraci korisni samo u otklanjanju poteškoća s uvjetnim pristupom značajke Azure Active Directory. Moguće je i karantensku napravu koja blokira pristup e-pošti putem pravilnika sustava Exchange. Dodatne informacije o upravljanju uređajima sustava Exchange možete pronaći [ovdje] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
