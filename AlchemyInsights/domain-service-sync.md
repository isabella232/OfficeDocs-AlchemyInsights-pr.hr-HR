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
ms.openlocfilehash: 95b5c3b768caf4b5d80a088a17a33facb39805fc766e4888586ae052d91681e3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057850"
---
# <a name="domain-service-synchronization"></a>Sinkronizacija servisa domene

Objekti i vjerodajnice u domeni Azure Active Directory Domain Services (Azure AD DS) mogu se stvoriti lokalno unutar domene ili sinkronizirati s klijenta servisa Azure Active Directory (Azure AD). Prilikom prve implementacije servisa Azure AD DS automatska se jednosmjestna sinkronizacija konfigurira i pokreće tako da replicira objekte sa servisa Azure AD. Ta jednosmjesna sinkronizacija i dalje se nastavlja izvoditi u pozadini da bi domena upravljanog servisa Azure AD DS bila autemna uz sve promjene servisa Azure AD. Sinkronizacija se ne odvija iz servisa Azure AD DS natrag na Azure AD.

Dodatne informacije o sinkronizaciji servisa Azure Active Directory domene potražite u članku [Sinkronizacija servisa domene](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization). 
