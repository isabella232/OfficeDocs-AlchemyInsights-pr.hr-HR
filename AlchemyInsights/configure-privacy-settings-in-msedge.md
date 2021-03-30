---
title: Konfiguriranje postavki zaštite privatnosti u pregledniku Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404376"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="d8f28-102">Konfiguriranje postavki zaštite privatnosti u pregledniku Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="d8f28-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="d8f28-103">Ako je Microsoft Edge implementiran na platformama koje nisu windows, dijagnostički podaci i podaci o web-mjestu po zadanom se ne šalju Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="d8f28-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="d8f28-104">No ako se Microsoft Edge implementiran u sustavu Windows 10, dijagnostički podaci i podaci o web-mjestu šalju se u skladu s korisničkim postavkama [dijagnostičkih podataka sustava Windows](https://go.microsoft.com/fwlink/?linkid=2132472).</span><span class="sxs-lookup"><span data-stu-id="d8f28-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="d8f28-105">Da biste konfigurirali način na koji Microsoft Edge upravlja prikupljanjem podataka za vašu organizaciju, koristite sljedeće pravilnike grupe:</span><span class="sxs-lookup"><span data-stu-id="d8f28-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="d8f28-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) uključuje izvješćivanje o korištenju i podacima povezanima s rušenjem.</span><span class="sxs-lookup"><span data-stu-id="d8f28-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="d8f28-107">[SendSiteInfoToImproveServices šalje informacije o](https://go.microsoft.com/fwlink/?linkid=2132470) web-mjestu koje se koriste za poboljšanje Microsoftovih servisa.</span><span class="sxs-lookup"><span data-stu-id="d8f28-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="d8f28-108">Dodatne informacije potražite u članku [Konfiguriranje postavki pravilnika](https://go.microsoft.com/fwlink/?linkid=2132577).</span><span class="sxs-lookup"><span data-stu-id="d8f28-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
