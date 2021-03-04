---
title: Praćenje neusklađeni uvjetni pristup
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427181"
---
# <a name="monitor-intune-conditional-access"></a>Praćenje neusklađeni uvjetni pristup

Korisnici usmjereni na uvjetni pristup primit će obavijest e-poštom ako ne zadovoljavaju preduvjete za pristup vaše tvrtke ili ustanove. Da biste riješili, preporučujemo vam jedno ili više sljedećih rješenja:

1. Ako se pretpostavlja da je uređaj upisan, savjetujte korisniku da otvori aplikaciju Portal tvrtke i provjerite prikazuje li se na portalu tvrtke. Ako to ne učinite, korisnik mora upisati uređaj.
1. **Na portalu** Azure potražite  >  **usklađenost uređaja**. 
1. Da biste pregledali izvješće o usklađenosti uređaja da biste provjerili je li korisnikov uređaj označenog kao kompatibilan, u odjeljku **Monitor** kliknite **usklađenost uređaja**.
1. **Na portalu** Azure potražite  >  **usklađenost uređaja**. U odjeljku **Upravljanje** kliknite **pravila**. Na popisu pravilnika o usklađenosti provjerite je li profil dodijeljen vašem korisničkom uređaju. Ako nijedan profil nije dodijeljen, zatim Intune neće moći potvrditi status usklađenosti uređaja.
1. Uredite korisnički zadatak uvjetnog pristupa.
1. Na portalu Azure prijeđite na **unos** pravilnika o  >  **uvjetnom pristupu**  >  , odaberite pravilo na popisu, a zatim kliknite **Korisnici i grupe**.
1. Da biste neku određenu politiku usmjerili na nekoga, dodajte ih na **popis uvrštavanje**. Da biste bili sigurni da je osoba izostavljena iz pravilnika, dodajte ih na **popis za izuzimanje**.

**Korisne veze:**

- [Pregled usklađenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Otklanjanje poteškoća sa com](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Pravilnik o otklanjanju poteškoća](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Praćenje usklađivanja uređaja](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Ovi su koraci korisni samo u otklanjanju poteškoća s uvjetnim pristupom značajke Azure Active Directory. Moguće je i karantensku napravu koja blokira pristup e-pošti putem pravilnika sustava Exchange. Dodatne informacije o upravljanju uređajima sustava Exchange možete pronaći [**ovdje**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
