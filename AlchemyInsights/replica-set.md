---
title: Skup replika
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713497"
---
# <a name="replica-set"></a>Skup replika

Dodatak se naziva i kao upravljana domena. To je zapravo dva kontrolora domene koji se pokreću i održavaju u pozadini. Dva DCs uključuju jedan glavni DC i jedan Replikacijski DC. Sigurnosne kopije u ZBRAJANJEM (upravljana domena) automatizirani su postupak koji upravlja platformom Azure. U slučaju problema s upravljanom domenom, Podrška za Azure može vam pomoći u vraćanju iz sigurnosne kopije.

Svaki skup replika stvarate u virtualnoj mreži. Svaka Virtualna mreža mora biti postavljena na svaku drugu virtualnu mrežu koja sadrži skup replika upravljanih domena. Ta konfiguracija stvara topologiju Mesh Network koja podržava replikaciju imenika. Virtualna mreža može podržavati višestruke skupove replika, pod uvjetom da je svaki skup replika u nekoj drugoj virtualnoj subnetu.

Dodatne informacije o skupu replika potražite u članku [Koncepti Skupovi replika](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
