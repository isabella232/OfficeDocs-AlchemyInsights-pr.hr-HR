---
title: rečeni kao ime datoteke je najbolji
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676525"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Obavezno Alkemija Zaglavlje H1, H2's ne rade.
Najbolje prakse i smjernice za alkemiju:

1. **Nemojte gnijezditi Alchemy Insights u mapama**- to će razbiti strukturu URL-a. Tražimo da ovo popravimo.
1. Datoteke u mapi **AlchemyInsights trebale** bi imati male nazive datoteka s crticama za razmakex. ***kako-to-omogućiti-parnica-hold.***
    1. Uključite ID pravila ili bucket S [portala Alchemy Partner](https://alchemyportal.azurewebsites.net) u polje ms.custom. Ex. ***ms.custom: 100021***
1. Ostale metapodatke pri vrhu ove datoteke koristite kao predložak.
1. Na [portalu Partner za alkemiju](https://alchemyportal.azurewebsites.net)idite na odjeljak **Naslov uvida korisnika:** i koristite to kao početnu točku za naslov H1 za uvid. 
    > [!NOTE]
    > Alkemija Insights MORA imati samo jedan H1 na vrhu ili će razbiti u proizvodnji. H2 s prikazom ni od njih koristite **podebljane** ili druge konvencije za označavanje zasebnih sekcija.
1. Zatim ispunite tijelo teksta pomoću skica materijala u odjeljku Uvidi korisnici na stranici Pravilo o upotrebi
    1. Popisi s grafičkim oznakama su u redu
    1. Numerirani popisi također
    1. **Podebljano** i *kurziv* je u redu.
    1. Linkovi bi uvijek trebali biti **"linkovi na web"/vanjske** ILI **dubinske veze na elemente korisničkog sučelja,** a ne interne veze.
    1. Slike trenutno nisu službeno podržane, ali je na planu.

A ovo je stvarno već malo predugo. Najbolja praksa je oko 400 znakova ---------------------------------

Nakon što je vaš sadržaj spreman, povucite ga u živu granu. Zatim idite na [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) i unesite naziv datoteke u polje URL-a. 