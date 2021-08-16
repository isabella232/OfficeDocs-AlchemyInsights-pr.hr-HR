---
title: Monitor Intune Conditional Access
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
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025494"
---
# <a name="monitor-intune-conditional-access"></a>Monitor Intune Conditional Access

Korisnici koji su ciljani uvjetnim pristupom primit će poruku e-pošte s obavijesti ako ne ispunjavaju preduvjete za pristup vašoj tvrtki ili ustanovi. Da biste riješili problem, preporučujemo jedno ili više sljedećih rješenja:

1. Ako se pretpostavlja da je uređaj upisan, savjetujte korisnika da ode u aplikaciju Company Portal i provjeri prikazuje li se u Company Portal. Ako se ne prijavi, korisnik mora registrirati uređaj.
1. Na portalu Azure idite na **usklađenost uređaja Intune**  >  . 
1. Da biste pogledali izvješće o usklađenosti uređaja da biste provjerili je li korisnikov uređaj označen kao usklađen, u **odjeljku Nadzor** kliknite **Usklađenost uređaja**.
1. Na portalu Azure idite na **usklađenost uređaja Intune**  >  . U **odjeljku Upravljanje** kliknite **Pravila**. Na popisu pravilnika o usklađenosti provjerite je li profil dodijeljen vašem korisničkom uređaju. Ako profil nije dodijeljen, Intune neće moći potvrditi status usklađenosti uređaja.
1. Uređivanje korisnikova zadatka uvjetnog pristupa.
1. Na portalu Azure otvorite **Intune**  >  **Pravila uvjetnog**  >  **pristupa**, odaberite pravilnik s popisa, a zatim kliknite Korisnici **i grupe**.
1. Da biste određeni pravilnik ciljali na nekoga, dodajte ga na **popis Uvrsti.** Da biste bili sigurni da je osoba izostavljena iz pravilnika, dodajte je na popis **Izuzimanje**.

**Korisne veze:**

- [Pregled usklađenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Otklanjanje poteškoća s ca](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Pravilnik o otklanjanju poteškoća](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Praćenje usklađenosti uređaja Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Ovi su koraci korisni samo u otklanjanju poteškoća Azure Active Directory uvjetnom pristupu. Uređaj koji blokira pristup e-pošti moguće je i staviti u karantenu pomoću pravilnika Exchange e-pošte. Dodatne informacije o upravljanju Exchange uređajima potražite [**ovdje**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
