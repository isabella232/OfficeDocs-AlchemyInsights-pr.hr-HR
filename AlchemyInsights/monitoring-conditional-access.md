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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975093"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Praćenje uvjetnog pristupa za Exchange

Korisnici koji su ciljani uvjetnim pristupom primit će poruku e-pošte s obavijesti ako ne ispunjavaju preduvjete za pristup vašoj tvrtki ili ustanovi. Da biste riješili problem, preporučujemo jedno ili više sljedećih rješenja:

- Ako se pretpostavlja da je uređaj upisan, savjetujte korisnika da ode u aplikaciju Company Portal i provjeri prikazuje li se u Company Portal. Ako se ne prijavi, korisnik bi trebao registrirati uređaj.
- Na portalu Azure idite na Intune > usklađenost uređaja. U odjeljku Nadzor kliknite Usklađenost uređaja. Pogledajte izvješće o usklađenosti uređaja da biste provjerili je li korisnikov uređaj označen kao usklađen.
- Na portalu Azure idite na Intune > usklađenost uređaja. U odjeljku Upravljanje kliknite Pravila. Na popisu pravilnika o usklađenosti provjerite je li profil dodijeljen vašem korisničkom uređaju. Ako profil nije dodijeljen, Intune neće moći potvrditi status usklađenosti uređaja.
- Uređivanje korisnikova zadatka uvjetnog pristupa.

1. Na portalu Azure idite na **Pravilnike uvjetnog pristupa za Intune**  >    >  .
2. Na popisu odaberite pravilnik.
3. Kliknite Korisnici i grupe.
4. Da biste određeni pravilnik ciljali na nekoga, dodajte ga na popis Uvrsti. Da biste bili sigurni da je osoba izostavljena iz pravilnika, dodajte je na popis Izuzimanje.

Korisne veze:

[Pregled usklađenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)

[Otklanjanje poteškoća s ca](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Pravilnik o otklanjanju poteškoća](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Praćenje usklađenosti uređaja Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Napomena: ovi su koraci korisni samo u otklanjanju poteškoća Azure Active Directory uvjetnom pristupu. Uređaj koji blokira pristup e-pošti moguće je i staviti u karantenu pomoću pravilnika Exchange e-pošte. Dodatne informacije o upravljanju Exchange uređajima možete pronaći [ovdje]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
