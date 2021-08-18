---
title: Microsoft Edge konfiguriranje postavki zaštite privatnosti
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114164"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge konfiguriranje postavki zaštite privatnosti

Ako se po zadanom Microsoft Edge na platformama koje nisu Windows, dijagnostički podaci i podaci o web-mjestu ne šalju se Microsoftu. No ako se Microsoft Edge u sustavu Windows 10, dijagnostički podaci i podaci o web-mjestu šalju se u skladu s [postavkama dijagnostičkih Windows korisnika](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

Da biste konfigurirali Microsoft Edge upravlja prikupljanjem podataka za vašu organizaciju, koristite sljedeće pravilnike grupe:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): ovim se pravilnikom omogućuje izvješćivanje o korištenju i podacima povezanima s rušenjem.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ovim se pravilnikom šalju podaci o web-mjestu koji se koriste za Microsoft services.

Dodatne informacije potražite u članku [Konfiguriranje postavki pravilnika](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).