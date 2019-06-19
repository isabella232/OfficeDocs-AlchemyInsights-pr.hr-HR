---
title: 2419 – nije moguće-za-Omogući-nadzor
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065613"
---
# <a name="unable-to-enable-unified-auditing"></a>Nije moguće omogućiti Objedinjena nadzor

Kada pokušate da omogućite Objedinjena nadzor za organizaciju Office 365, možda ćete primiti pogrešku sličnu sljedeće:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Da biste riješili taj problem, slijedite ove korake:

1. [Povezivanje s Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Pokrenite cmdlet sljedeće:

   ```
   Enable-OrganizationCustomization
   ```

3. Pričekajte 60 minuta prethodne postavke stupile na snagu.

4. U Exchange Online PowerShell pokrenite sljedeću naredbu:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Dodatne informacije potražite u sljedećim člancima:

- [Povezivanje s Exchange Online PowerShell pomoću višestruku provjeru autentičnosti](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Uključivanje ili isključivanje pretraživanje zapisnika nadzora za Office 365](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
