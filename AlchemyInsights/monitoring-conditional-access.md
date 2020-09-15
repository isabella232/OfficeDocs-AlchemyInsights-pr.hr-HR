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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702895"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Praćenje uvjetnog pristupa za Exchange

Korisnici usmjereni na uvjetni pristup primit će obavijest e-poštom ako ne zadovoljavaju preduvjete za pristup vaše tvrtke ili ustanove. Da biste riješili, preporučujemo vam jedno ili više sljedećih rješenja:
  
- Ako se pretpostavlja da je uređaj upisan, savjetujte korisniku da otvori aplikaciju Portal tvrtke i provjerite prikazuje li se na portalu tvrtke. Ako se to ne dogodi, korisnik bi trebao upisati uređaj.
    
- Na portalu Azure potražite ** \> usklađenost uređaja**. U odjeljku **Monitor** kliknite **usklađenost uređaja**. Prikažite izvješće o usklađenosti uređaja da biste provjerili je li korisnikov uređaj označenog kao usklađen. 
    
- Na portalu Azure potražite ** \> usklađenost uređaja**. U odjeljku **Upravljanje**kliknite **pravila**. Na popisu pravilnika o usklađenosti provjerite je li profil dodijeljen vašem korisničkom uređaju. Ako nijedan profil nije dodijeljen, zatim Intune neće moći potvrditi status usklađenosti uređaja. 
    
- Uredite korisnički zadatak uvjetnog pristupa.
    
1. Na portalu Azure idite na umetanje **pravilnika o \> uvjetnom \> pristupu**
    
2. Odabir pravilnika s popisa
    
3. Kliknite **Korisnici i grupe**
    
4. Da biste neku određenu politiku usmjerili na nekoga, dodajte ih na popis **uvrštavanje** . Da biste bili sigurni da je osoba izostavljena iz pravilnika, dodajte ih na popis za **izuzimanje** . 
    
Pročitajte više: [Praćenje uređaja za uvjetni pristup](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

