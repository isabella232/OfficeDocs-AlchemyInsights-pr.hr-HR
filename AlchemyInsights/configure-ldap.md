---
title: Konfiguriranje LDAP-a
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
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090404"
---
# <a name="configure-ldap"></a>Konfiguriranje LDAP-a

Da biste konfigurirali LDAP, učinite sljedeće:

1. Provjerite stanje domene na [portalu Azure](https://aka.ms/aadds-health).
1. Provjerite je li dostupna valjana pretplata na Azure AD i je li omogućen servis Azure AD Domain Services.
1. Certifikat potreban za omogućivanje sigurnog LDAP-a mora biti dobiven od pouzdane javne ustanove za izdavanje certifikata ili biti samoispunjavanje certifikata.
1. Provjerite je li certifikat u skladu s [obaveznim smjernicama](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Certifikat nije valjan**
1. Da biste obnovili certifikat, slijedite korake za stvaranje novog certifikata i ponovno učitavanje: [Konfiguriranje LDAP-a.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Da biste riješili poznati problem sa sigurnosnim LDAP upozorenjima u servisu Azure Active directory Domain Services, pogledajte [razrješavanje LDAP upozorenja](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
