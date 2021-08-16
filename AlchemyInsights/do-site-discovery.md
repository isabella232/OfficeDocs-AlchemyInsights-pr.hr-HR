---
title: Otkrivanje web-mjesta
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030750"
---
# <a name="do-site-discovery"></a>Otkrivanje web-mjesta

Ako vaša tvrtka ili ustanova i dalje koristi naslijeđene web-aplikacije i tarife za korištenje načina rada preglednika Internet Explorer (što većina korisnika radi), trebali biste učiniti još nekih dodatnih otkrivanja web-mjesta.

**Već ste implementirati stariju verziju sustava Microsoft Edge**

Ako ste već konfigurirali popis enterprise web-mjesta tako da funkcionira za naslijeđenu verziju Microsoft Edge, otkrivanje web-mjesta gotovo je gotovo. Možda ćete morati dodati neutralna web-mjesta.

Neutralna web-mjesta obično su web-mjesta koja pružaju jedinstvenu prijavu (SSO). Ako s web-mjesta Microsoft Edge neutralno web-mjesto, želite ostati Microsoft Edge provjeru autentičnosti. Ako u načinu rada preglednika Internet Explorer otvorite neutralno web-mjesto, želite ostati u načinu rada preglednika Internet Explorer da biste provjerili autentičnost.

Odredite SSO ili druga neutralna web-mjesta koja koristite i dodajte ih na popis enterprise web-mjesta.

**Internet Explorer zadani je preglednik**

Ako sada koristite samo Internet Explorer, možda ne znate koja su web-mjesta nadograđena na moderne web-standarde i koja i dalje zahtijevaju Internet Explorer. Te ćete web-mjesta morati pronaći i dodati na popis enterprise web-mjesta da biste mogli koristiti način rada preglednika Internet Explorer samo za ta web-mjesta.

> [!NOTE]
> [Otkrivanje enterprise web-mjesta](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) otkriva web-mjesta koja bi mogla zatrebati način rada preglednika Internet Explorer. Može prikupljati podatke na računalima Windows Internet Explorer 8 putem preglednika Internet Explorer 11 na Windows 10, Windows 8.1 ili Windows 7.

**Analiza podataka**

Kada prikupite podatke web-mjesta, preporučujemo sljedeći postupak u četiri koraka za analizu podataka:
1. Sortiraj podatke po domeni, a zatim prema URL-u.
2. Definirajte granice aplikacije koju želite konfigurirati za način rada preglednika Internet Explorer. Želite uvrstiti sva web-mjesta i web-kontrole koje definiraju aplikaciju, ali ne želite uvrstiti dodatna web-mjesta i kontrole. Neka web-mjesta mogu biti jednostavna kao *https://contoso.com/app1* i druga web-mjesta, dok drugi moraju definirati više web-mjesta i stranica.
3. Testirajte aplikaciju da biste provjerili ne funkcionira li nativno. Mnoga će web-mjesta ponuditi moderni sadržaj kada otkriju moderni preglednik i nude naslijeđeni sadržaj samo kada otkriju Internet Explorer.
4. Dodajte aplikaciju na popis enterprise web-mjesta ako ne uspije testirati.

> [!NOTE]
> Kao najbolje prakse grupirajte sva web-mjesta koja obuhvaćaju aplikaciju. Na taj način, prilikom nadogradnje aplikacije, lakše je ukloniti cijelo web-mjesto iz načina rada preglednika Internet Explorer i početi koristiti moderni preglednik za tu aplikaciju.

Kada završite s otkrivanjem web-mjesta i analizirate podatke, spremni ste početi gledati strategiju kanala.

