---
title: Office 2019 na terminalskom poslužitelju ili RDS-u
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3487"
- "9001419"
ms.openlocfilehash: 3b61f0396c4698aaa54df74d6612d1a35d37f652
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790972"
---
# <a name="deploying-office-2019-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="359c2-102">Implementacija sustava Office 2019 za zajedničko korištenje na servisima RDS, Terminal Server ili VDI</span><span class="sxs-lookup"><span data-stu-id="359c2-102">Deploying Office 2019 for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="359c2-103">Ako je Office već instaliran na RDS poslužitelju pomoću bilo koje druge tarife sustava Office, deinstalirajte ga.</span><span class="sxs-lookup"><span data-stu-id="359c2-103">If Office is already installed on the RDS server using any other Office plans, uninstall it.</span></span> <span data-ttu-id="359c2-104">Na primjer, idite na **Upravljačka**  >  **ploča Deinstaliranje programa**.</span><span class="sxs-lookup"><span data-stu-id="359c2-104">For example, go to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="359c2-105">Ako nailazite na probleme, deinstalirajte pomoću Microsoftova [pomoćnika za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="359c2-105">If you're experiencing issues, uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span></span> 

<span data-ttu-id="359c2-106">Instalirajte Office pomoću alata za implementaciju sustava Office (ODT).</span><span class="sxs-lookup"><span data-stu-id="359c2-106">Use the Office Deployment Tool (ODT) to install Office.</span></span> <span data-ttu-id="359c2-107">Detaljne korake potražite u članku [Implementacija sustava Office 2019](https://docs.microsoft.com/deployoffice/office2019/deploy).</span><span class="sxs-lookup"><span data-stu-id="359c2-107">For detailed steps, see [Deploy Office 2019](https://docs.microsoft.com/deployoffice/office2019/deploy).</span></span>

<span data-ttu-id="359c2-108">Aktivaciju potražite u članku [Pregled količinske aktivacije sustava Office](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office).</span><span class="sxs-lookup"><span data-stu-id="359c2-108">For activation, see [Overview of volume activation of Office](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office).</span></span>