---
title: EndPoint Manager – sigurnosne osnovne vrijednosti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420719"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – sigurnosne osnovne vrijednosti

Sigurnosne su osnovne vrijednosti unaprijed konfigurirane grupe postavki sustava Windows koje vam pomažu pri primjeni sigurnosnih postavki koje preporučuju odgovarajući sigurnosni timovi. Te se osnovne vrijednosti mogu prilagoditi tako da se isporučuju samo željene postavke i vrijednosti. Dodatne informacije o sigurnosnim osnovnim vrijednostima potražite u članku Konfiguriranje uređaja sa sustavom [Windows 10 pomoću sigurnosnih osnova u aplikaciji Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Trenutno postoje osnovne vrijednosti za ove proizvode:

- Postavke sigurnosti MDM-a u sustavu Windows
- Microsoft Defender for EndPoint Security
- Microsoft Edge

Svaka od osnovnih vrijednosti ažurira se povremeno i ispušta u inkrementalnim verzijama. Svaka verzija dodaje i uklanja postavke iz prethodne verzije da bi osnovna vrijednost zadovoljavala trenutne smjernice. Konzola Sigurnosne osnovne vrijednosti u sigurnosti krajnjih točaka omogućuje uspoređenje različitih verzija tako da se promjene iz verzije u verziju uspoređuju vidljivima.

Upute za učinkovitu promjenu verzije osnovne vrijednosti potražite u članku Upravljanje sigurnosnim osnovnim [profilima u aplikaciji Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Nakon implementacije sigurnosne osnovice možete pratiti stanje implementacije i pregledati postavke na temelju uređaja po uređaj.

**Napomena:** Podaci za izvješćivanje o osnovnim vrijednostima mogu potrajati do 24 sata da bi se pojavili od početne implementacije na uređaj i do 6 sati radi dodatnih ažuriranja. 

Najčešći uzrok ne primjenjuje se osnovna postavka jer se ista postavka koristi u drugom profilu. Taj se scenarij može istražiti za određeni uređaj tako da odaberete taj uređaj u sklopu sustava Status uređaja profila sigurnosne osnovice. Detalje potražite u članku [Razrješavanje sukoba za sigurnosne osnovne vrijednosti](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).