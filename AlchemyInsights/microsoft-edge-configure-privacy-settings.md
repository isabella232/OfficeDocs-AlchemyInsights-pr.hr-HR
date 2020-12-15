---
title: Konfiguriranje postavki zaštite privatnosti u pregledniku Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676973"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="72c81-102">Konfiguriranje postavki zaštite privatnosti u pregledniku Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="72c81-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="72c81-103">Prema zadanim postavkama, ako je Microsoft Edge raspoređen na platforme koje nisu Windows, dijagnostički podaci i podaci o web-mjestu ne šalju se Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="72c81-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="72c81-104">No ako je Microsoft Edge raspoređen u sustavu Windows 10, dijagnostički podaci i podaci o web-mjestu šalju se u skladu s [postavkama dijagnostičkih podataka korisnika sustava Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="72c81-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="72c81-105">Da biste konfigurirali način na koji Microsoft Edge rukuje zbirkom podataka za vašu tvrtku ili ustanovu, poslužite se sljedećim pravilima grupe:</span><span class="sxs-lookup"><span data-stu-id="72c81-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="72c81-106">[Metricsreportingenabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): u ovom se pravilniku omogućuje izvješćivanje o korištenju i podacima koji se odnose na rušenje.</span><span class="sxs-lookup"><span data-stu-id="72c81-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="72c81-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): ovo pravilo šalje informacije o web-mjestu koje se koriste za unaprjeđenje Microsoftovih servisa.</span><span class="sxs-lookup"><span data-stu-id="72c81-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="72c81-108">Dodatne informacije potražite u članku [Konfiguriranje postavki pravilnika](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="72c81-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>