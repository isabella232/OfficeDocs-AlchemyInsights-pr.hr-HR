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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="0e2d6-102">Nije moguće omogućiti Objedinjena nadzor</span><span class="sxs-lookup"><span data-stu-id="0e2d6-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="0e2d6-103">Kada pokušate da omogućite Objedinjena nadzor za organizaciju Office 365, možda ćete primiti pogrešku sličnu sljedeće:</span><span class="sxs-lookup"><span data-stu-id="0e2d6-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="0e2d6-104">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="0e2d6-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="0e2d6-105">[Povezivanje s Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="0e2d6-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="0e2d6-106">Pokrenite cmdlet sljedeće:</span><span class="sxs-lookup"><span data-stu-id="0e2d6-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="0e2d6-107">Pričekajte 60 minuta prethodne postavke stupile na snagu.</span><span class="sxs-lookup"><span data-stu-id="0e2d6-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="0e2d6-108">U Exchange Online PowerShell pokrenite sljedeću naredbu:</span><span class="sxs-lookup"><span data-stu-id="0e2d6-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="0e2d6-109">Dodatne informacije potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="0e2d6-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="0e2d6-110">Povezivanje s Exchange Online PowerShell pomoću višestruku provjeru autentičnosti</span><span class="sxs-lookup"><span data-stu-id="0e2d6-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="0e2d6-111">Uključivanje ili isključivanje pretraživanje zapisnika nadzora za Office 365</span><span class="sxs-lookup"><span data-stu-id="0e2d6-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
