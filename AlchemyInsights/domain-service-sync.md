---
title: Sinkronizacija servisa domene
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884844"
---
# <a name="domain-service-synchronization"></a>Sinkronizacija servisa domene

Objekti i vjerodajnice u upravljanoj domeni servisa Azure Active Directory (Azure AD DS) mogu se stvarati lokalno unutar domene ili sinkronizirati iz korisnika Azure Active Directory (Azure AD). Kada prvi put implementirate Azure AD DS, konfigurirajte jednosmjernu sinkronizaciju, a zatim pokrenete da biste replicirali objekte iz servisa Azure AD. Ovaj jednosmjerna sinkronizacija nastavlja se pokretati u pozadini da bi se u servisu Azure AD domogla ažurirane domene s promjenama iz Azure AD. Nema sinkronizacije iz servisa Azure AD DS natrag na Azure AD.

Dodatne informacije o sinkronizaciji servisa Azure Active Directory domena potražite u članku [Sinkronizacija servisa domene](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization). 
