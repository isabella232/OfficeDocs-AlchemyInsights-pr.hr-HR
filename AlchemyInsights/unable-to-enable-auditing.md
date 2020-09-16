---
title: 2419 – revizija nije moguće omogućiti-
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
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767591"
---
# <a name="unable-to-enable-unified-auditing"></a>Nije moguće omogućiti ujedinjenje nadzora

Kada pokušate omogućiti sjedinjeno nadziranje tvrtke ili ustanove, možda će vam se prikazati pogreška slična sljedećoj:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Da biste riješili taj problem, slijedite ove korake:

1. [Spojite se na PowerShell sustava Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Pokrenite sljedeći cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Pričekajte 60 minuta da bi Prethodna postavka stupila na kraj.

4. Pokrenite sljedeću naredbu u komponenti Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Dodatne informacije potražite u sljedećim člancima:

- [Spojite se na komponente Exchange Online PowerShell pomoću multi-Factor provjera autentičnosti](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Uključivanje i isključivanje pretraživanja zapisnika nadzora](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
