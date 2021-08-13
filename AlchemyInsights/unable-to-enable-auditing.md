---
title: 2419-unable-to-enable-auditing
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007782"
---
# <a name="unable-to-enable-unified-auditing"></a>Nije moguće omogućiti sjedinjeno nadziranje

Kada pokušate omogućiti sjedinjeni nadzor za svoju organizaciju, može vam se pojaviti pogreška slična sljedećoj:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Da biste riješili taj problem, slijedite ove korake:

1. [Povezivanje na Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Pokrenite sljedeći cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Pričekajte 60 minuta da bi prethodna postavka snazi.

4. Pokrenite sljedeću naredbu u Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Dodatne informacije potražite u sljedećim člancima:

- [Povezivanje za Exchange Online PowerShell pomoću višestruke provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Uključivanje i isključivanje pretraživanja zapisnika nadzora](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
