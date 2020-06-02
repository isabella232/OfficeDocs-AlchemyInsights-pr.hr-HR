---
title: revizije koja nije u mogućnosti omogućiti
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510420"
---
# <a name="unable-to-enable-unified-auditing"></a>Nije moguće omogućiti objedinjeno nadziranje

Kada pokušate omogućiti objedinjeno nadziranje za svoju tvrtku ili ustanovu, možda ćete primiti pogrešku sličnu sljedećoj:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Da biste riješili taj problem, slijedite ove korake:

1. [Povezivanje sa ljuskom PowerShell sustava Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Trčanje slijedeće cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Pričekajte 60 minuta da prethodna postavka stupiti na snagu.

4. Pokrenite sljedeću naredbu u dodatku PowerShell sustava Exchange Online:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Dodatne informacije potražite u sljedećim člancima:

- [Povezivanje sa sustavom Exchange Online PowerShell pomoću višestruke provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Uključivanje i isključivanje pretraživanja zapisnika nadzora](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
