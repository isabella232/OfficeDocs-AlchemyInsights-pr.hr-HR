---
title: isti kao naziv datoteke je najbolje
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 5555
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 68f743ee9c448565470815f8410cc6ce4b384bed
ms.sourcegitcommit: 0b6e9470c6b73616ba8bacef7010f739b7fac332
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/21/2019
ms.locfileid: "30742370"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Potrebna alkemiji zaglavlje H1, H2's ne rade.
Najbolje prakse i smjernice za autorizaciju alkemiji:

1. **Ugnijezditi alkemiji uvida u mapama**- će ovo prelomiti strukturu url. Možemo traženu u popravljanju to.
1. Datoteke u mapi **AlchemyInsights** treba imati malo nazivi datoteka s spojnice razmake prije. ***how-to-Omogući-sudskih procesa-drži***.
    1. ID pravila ili bucket ID iz [alkemiji partnera portala](https://alchemyportal.azurewebsites.net) uključiti u polje ms.custom. Franko. ***MS.Custom: 100021***
1. Koristite ostatak metapodatke na vrhu ovu datoteku kao predložak.
1. U [alkemiji partnera portal](https://alchemyportal.azurewebsites.net)pronađite odjeljak **Naslov uvid kupca:** i korištenje koji kao početni pokažite za H1 naslov na uvid. 
    > [!NOTE]
    > Alkemiji uvide mora imati samo jednu H1 na vrhu ili će prekinuti u proizvodnji. H2s ne renderirati tako koristi **Podebljano** ili druge konvencije za naznaku zasebnim sekcijama.
1. Dalje, ispunite tijelo teksta pomoću materijala skice u sekciji kupca uvide pravilo alkemiji stranice
    1. Popisi s grafičkim oznakama su precizno
    1. Previše numeriranih popisa
    1. **Podebljano** i *kurziv* su a-ok
    1. Veze uvijek mora biti ili **"veze web" / vanjski** ili **dublje veze elemenata korisničkog Sučelja**, ne i interne veze.
    1. Slike su službeno nije podržana u ovom trenutku, ali ga je u roadmap.

I to je zaista već je malo predugačak. Najbolje je o 400 znakova---

Kada vaš sadržaj bude spremna, istaknuti ga uživo granu. Zatim idite na [portal alkemiji partnera](https://alchemyportal.azurewebsites.net) i unesite naziv datoteke u polje url. M