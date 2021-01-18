---
title: Virtualna konfiguracija s servisima AAD domene
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884857"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtualna konfiguracija s servisima AAD domene

Virtualna konfiguracija uz usluge AAD domene obuhvaća sljedeće korake: 

1. Provjeru zdravlja domene na portalu Azure https://aka.ms/aadds-health
2. Provjeru programa NSG za pravila koja blokiraju priključke potrebne za sinkronizaciju na servisu Azure AD domene na portalu https://aka.ms/aadds-networking
3. Osiguravanje da je Virtualna mreža raspoređena u istoj regiji Azure kao domena servisa Azure AD
4. Osiguravanje da nemate postojeću domenu s istim nazivom domene dostupnom na virtualnoj mreži.

Dodatne informacije o prikazu dizajna na virtualnoj mreži Azure za podršku servisima AAD domene potražite u članku [razmatranje virtualne mreže](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

