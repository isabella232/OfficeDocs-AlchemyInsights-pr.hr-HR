---
title: 'isti kao naziv datoteke je najbolje [pravilo #-opis]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662922"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a>Potreban klijent nasuprotne H1, H2 ne radi
Primjer teksta Blokiraj - slijedite ove upute:

1. Datoteke u mapi **AlchemyInsights** treba imati pravilo ID i naziv pravila s [portala alkemiji partnera](https://alchemyportal.azurewebsites.net) u naziv datoteke.
    1. Ex. ***976-How-to-enable-litigation-hold***
1. Koristite metapodatke na vrhu ovu datoteku kao predložak. Ništa drugo nije potrebna.
1. U [alkemiji partnera portal](https://alchemyportal.azurewebsites.net)pronađite odjeljak **Naslov uvid kupca:** i korištenje koji kao početni pokažite za H1 naslov na uvid. 
    > [!NOTE]
    > Alkemiji uvide mora imati samo jednu H1 na vrhu ili će prekinuti u proizvodnji. H2s ne renderirati tako koristi **Podebljano** ili druge konvencije za naznaku zasebnim sekcijama.
1. Dalje, ispunite tijelo teksta pomoću materijala skice u sekciji kupca uvide pravilo alkemiji stranice
    1. Popisi s grafičkim oznakama su precizno
    1. Previše numeriranih popisa
    1. **Podebljano** i *kurziv* su a-ok
    1. Veze uvijek mora biti ili **"veze web" / vanjski** ili **dublje veze elemenata korisničkog Sučelja**, ne i interne veze.

I to je zaista već je malo predugačak. Najbolje je o 400 znakova---

Kada vaš sadržaj bude spremna, istaknuti ga uživo granu. Zatim idite na [portal alkemiji partnera](https://alchemyportal.azurewebsites.net) i unesite naziv datoteke u polje url. Provjerite uvid pregledavaju i objavljuju kaže "da", a zatim kliknite pravilo ažuriranja. (To će izgledati prettier u novu verziju portala - otpustite uskoro.)

![URL polje](media/for-content-team.PNG)

