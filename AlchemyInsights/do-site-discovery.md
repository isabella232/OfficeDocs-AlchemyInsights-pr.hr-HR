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
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692671"
---
# <a name="do-site-discovery"></a>Otkrivanje web-mjesta

Ako vaša tvrtka ili ustanova još uvijek koristi naslijeđene web-aplikacije i planira koristiti način rada u pregledniku Internet Explorer (što većina kupaca radi), trebali biste učiniti dodatna otkrića web-mjesta.

**Već ste implementirali stariju verziju sustava Microsoft Edge**

Ako ste već konfigurirali popis web-mjesta tvrtke da funkcionira za naslijeđenu verziju sustava Microsoft Edge, otkriće web-mjesta gotovo je dovršeno. Možda ćete morati dodati neutralna web-mjesta.

Neutralna web-mjesta obično su web-mjesta koja sadrže jedinstvenu prijavu (SSO). Ako odete na neutralno web-mjesto iz programa Microsoft Edge, želite biti autentificiraj u pregledniku Microsoft Edge. Ako u načinu rada Internet Explorera odete na neutralno web-mjesto, u načinu rada u pregledniku Internet Explorer želite biti autentificiraj.

Odredite bilo koje SSO ili druga neutralna web-mjesta koja koristite i dodajte ih na popis web-mjesta tvrtke.

**Internet Explorer zadani je preglednik**

Ako trenutno koristite Internet Explorer, možda nećete znati koje su web-mjesta nadogradili na moderne web-standarde i za koje je i dalje potreban Internet Explorer. Te web-mjesta želite pronaći i dodati na popis Enterprise web-mjesta da biste mogli koristiti način rada u pregledniku Internet Explorer samo za ta web-mjesta.

> [!NOTE]
> [Otkriće web-mjesta Enterprise](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) otkriva web-mjesta koja možda trebaju način rada preglednika Internet Explorer. Može prikupljati podatke na računalima sa sustavom Windows Internet Explorer 8 putem preglednika Internet Explorer 11 u sustavima Windows 10, Windows 8,1 ili Windows 7.

**Analiziranje podataka**

Kada prikupite podatke web-mjesta, preporučujemo sljedeći postupak u četiri koraka radi analize podataka:
1. Sortirajte podatke prema domeni, a zatim prema URL-u.
2. Definiranje granica aplikacije za konfiguriranje načina rada u pregledniku Internet Explorer. Želite uvrstiti sva web-mjesta i web-kontrole koje definiraju aplikaciju, ali ne želite uvrstiti dodatna web-mjesta i kontrole. Neka web-mjesta mogu biti jednostavna kao i *https://contoso.com/app1* dok bi drugi mogli zahtijevati definiranje više web-mjesta i stranica.
3. Testirajte aplikaciju da biste potvrdili da ne funkcionira u urođenom. Mnoga će web-mjesta ponuditi moderan sadržaj kada otkriju moderan preglednik i nude samo naslijeđeni sadržaj kada otkriju Internet Explorer.
4. Dodajte aplikaciju na popis web-mjesta tvrtke ako ne uspije testirati.

> [!NOTE]
> Kao najbolju praksu grupirajte sva web-mjesta koja sadrže aplikaciju. Na taj način, kada nadogradite aplikaciju, lakše je ukloniti cijelo web-mjesto iz načina rada Internet Explorer i početi koristiti moderan preglednik za tu aplikaciju.

Kada završite s otkrivanjem web-mjesta i analizirali ste podatke, spremni ste početi gledati strategiju kanala.

