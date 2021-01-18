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
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884845"
---
# <a name="configure-ldap"></a>Konfiguriranje LDAP-a

Da biste konfigurirali LDAP, učinite sljedeće:

1. Provjerite zdravlje domene na [portalu Azure](https://aka.ms/aadds-health).
1. Provjerite je li dostupna valjana pretplata na Azure AD, a omogućen je i Azure AD Domain Services.
1. Certifikat potreban za omogućavanje sigurnog LDAP-a mora biti dobiven od pouzdanih javnih ustanova za izdavanje certifikata ili biti samopotpisani certifikat.
1. Uvjerite se da certifikat slijedi potrebne [smjernice](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Potvrda nije valjana**
1. Da biste obnovili certifikat, slijedite korake za stvaranje novog certifikata i Reupload: [Konfigurisanje LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)-a.
1. Da biste riješili poznat problem s sigurnim LDAP upozorenjima u domenama servisa Azure Active Directory, pročitajte članak [rješavanje LDAP upozorenja](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
