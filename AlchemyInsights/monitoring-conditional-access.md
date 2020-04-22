---
title: Praćenje uvjetnog pristupa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713710"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Praćenje uvjetnog pristupa za Exchange

Korisnici koji ciljaju s uvjetnim pristupom primit će e-poruku s obavijesti ako ne ispunjavaju zahtjeve pristupa vaše tvrtke ili ustanove. Da biste riješili problem, preporučujemo jedno ili više sljedećih rješenja:
  
- Ako se pretpostavlja da je uređaj upisan, obavijestite korisnika da ode u aplikaciju Portal tvrtke i provjeri pojavljuje li se na portalu tvrtke. Ako se to ne dogodi, korisnik bi trebao upisati uređaj.
    
- Na portalu Azure idite na **usklađenost uređaja Intune \> **. U **odjeljku Monitor** kliknite **Usklađenost uređaja**. Pregledajte izvješće o usklađenosti uređaja da biste provjerili je li korisnikov uređaj označen kao sukladan. 
    
- Na portalu Azure idite na **usklađenost uređaja Intune \> **. U **odjeljku Upravljanje**kliknite **Pravila**. Na popisu pravila o usklađenosti provjerite je li profil dodijeljen uređaju vašeg korisnika. Ako profil nije dodijeljen, Intune neće moći potvrditi status usklađenosti uređaja. 
    
- Uredite korisnikovu dodjelu uvjetnog pristupa.
    
1. Na portalu Azure idite na **Pravila uvjetnog pristupa \> \> Podešavanja**
    
2. Odabir pravila s popisa
    
3. Kliknite **Korisnici i grupe**
    
4. Da biste ciljali određena pravila kod nekoga, dodajte ih na popis **Uključi.** Da biste osigurali da je osoba izostavljena iz pravila, dodajte je na popis **Izuzima.** 
    
Opširnije: [Kako nadzirati uređaje uvjetnog pristupa](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

