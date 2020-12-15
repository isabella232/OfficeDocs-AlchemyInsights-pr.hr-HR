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
# <a name="microsoft-edge-configure-privacy-settings"></a>Konfiguriranje postavki zaštite privatnosti u pregledniku Microsoft Edge

Prema zadanim postavkama, ako je Microsoft Edge raspoređen na platforme koje nisu Windows, dijagnostički podaci i podaci o web-mjestu ne šalju se Microsoftu. No ako je Microsoft Edge raspoređen u sustavu Windows 10, dijagnostički podaci i podaci o web-mjestu šalju se u skladu s [postavkama dijagnostičkih podataka korisnika sustava Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

Da biste konfigurirali način na koji Microsoft Edge rukuje zbirkom podataka za vašu tvrtku ili ustanovu, poslužite se sljedećim pravilima grupe:
- [Metricsreportingenabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): u ovom se pravilniku omogućuje izvješćivanje o korištenju i podacima koji se odnose na rušenje.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): ovo pravilo šalje informacije o web-mjestu koje se koriste za unaprjeđenje Microsoftovih servisa.

Dodatne informacije potražite u članku [Konfiguriranje postavki pravilnika](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).