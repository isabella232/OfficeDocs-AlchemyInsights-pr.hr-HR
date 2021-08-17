---
title: isto kao i naziv datoteke je najbolji
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312817"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Obavezno zaglavlje alkemije H1, H2 ne funkcionira".
Najbolje prakse i smjernice za alkemiju:

1. **Nemojte ugnijezditi Alchemy Uvidi u mape**– time ćete prekinuti strukturu URL-a. Radimo na rješavanju ovog problema.
1. Datoteke u mapi **AlchemyInsights** moraju imati mala slova s crticama za razmake ex. **_how-to-enable-litigation-hold_**.
    1. U polje ms.custom uvrsti ID pravila ili ID ćelije s portala Partnera za [Alchemy.](https://alchemyportal.azurewebsites.net) ex. ***ms.custom: 100021***
1. Ostatak metapodataka pri vrhu datoteke koristite kao predložak.
1. Na [portalu Alchemy Partner](https://alchemyportal.azurewebsites.net)pomaknite se prema dolje do odjeljka Naslov uvida u **klijente:** i upotrijebite ga kao početnu točku za naslov H1 za uvid. 

**Napomena:** Alchemy Uvidi mora imati samo jedan H1 pri vrhu ili će se prekinuti u produkciji. H2s ne renderirati bilo na taj način koristite **podebljano** ili druge konvencije za potpisivanje zasebnih sekcija.
1. Zatim ispunite tijelo teksta pomoću materijala skice u odjeljku Customer Insights na stranici Pravila alkemije
    1. Popisi s grafičkim oznakama su u redu
    1. Numerirani popisi
    1. **Bold** and *italic* are a-ok
    1. Veze moraju uvijek biti "veze na **web"/vanjske** ili dubinske veze na elemente **sučelja,** a ne interne veze.
    1. Slike u ovom trenutku nisu službeno podržane, ali su na putu.

A to je već predugo. Najbolja praksa je oko 400 znakova ---------------------------------

Kada sadržaj bude spreman, povucite ga na ogranak uživo. Zatim idite na [portal Partnera za Alchemy i](https://alchemyportal.azurewebsites.net) unesite naziv datoteke u polje URL- a. 