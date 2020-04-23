---
title: 932 Nadogradnja AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766485"
---
# <a name="upgrade-azure-ad-connect"></a>Nadogradnja usluge Azure AD Connect

Prema zadanim postavkama, automatska nadogradnja omogućena je za Azure AD Connect, čime se osigurava da koristite najnoviju verziju. Da biste provjerili postavke automatske nadogradnje, koristite cmdlet **Get-ADSyncAutoUpgrade** u Azure AD PowerShell. Cmdlet će vratiti jednu od sljedećih vrijednosti:

- **Omogućeno**: Omogućena je automatska nadogradnja.

- **Onemogućeno:** Automatska nadogradnja je onemogućena.

- **Obustavljeno:** sustav više ne ispunjava uvjete za primanje automatskih nadogradnji. Tu vrijednost ne možete konfigurirati; To je postavljen od strane sustava.

Dodatne informacije potražite u [odjeljku Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Da biste preuzeli najnoviju verziju [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)usluge Azure AD Connect, idite na .
