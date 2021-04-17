---
title: Promjena poslužitelja naziva
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818604"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Ažuriranje poslužitelja naziva u vašoj domeni da bi upućivali na Microsoft

Napomena: propagiranje promjena poslužitelja naziva ponekad može potrajati do 48 sati.
  
Da biste postavili domenu u okruženju Microsoft 365, moraju se ažurirati poslužitelji naziva pri registraru. Stvorite ili uredite zapise poslužitelja naziva pri registraru domene.
  
1. Idite na web-mjesto registrara domene i potražite područje u kojemu možete urediti poslužitelje naziva.
  
2. Stvorite ili uredite dva zapisa poslužitelja naziva tako da odgovaraju ovim vrijednostima:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Spremite promjene.

Detaljne upute možete pronaći i u ovom članku: [Promjena poslužitelja naziva pri registraru domene](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  