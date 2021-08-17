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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110672"
---
# <a name="replica-set"></a>Skup replika

AADDS se naziva i kao upravljana domena. To su zapravo dva kontrolora domena koja se vode i održavaju u stražnjem domenu. Dva DC-a obuhvaćaju jedan glavni DC i jednu replikaciju DC- a. Sigurnosne kopije u AADDS-u (upravljana domena) automatizirani su proces kojim upravlja platforma Azure. U slučaju problema s upravljanom domenom podrška za Azure može vam pomoći u vraćanju iz sigurnosne kopije.

Svaku repliku stvarate u virtualnoj mreži. Svaka virtualna mreža mora biti ravnopravna sa svakom drugom virtualnom mrežom koja hostira skup replika upravljane domene. Ta konfiguracija stvara mrežnu topologiju mreže koja podržava replikaciju direktorija. Virtualna mreža može podržavati više skupova replika, pod uvjetom da se svaki skup replika nalazi na drugoj virtualnoj podmreži.

Dodatne informacije o skupu replika potražite u članku [Skupovi replika koncepta](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
