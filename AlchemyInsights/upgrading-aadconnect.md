---
title: 932 Nadogradnja AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104804"
---
# <a name="upgrade-azure-ad-connect"></a>Nadogradnja servisa Azure AD Povezivanje

Automatska je nadogradnja po zadanom omogućena za Azure AD Povezivanje, što pridonosi tome da koristite najnoviju verziju. Da biste provjerili postavke **automatske nadogradnje, koristite cmdlet Get-ADSyncAutoUpgrade** u ljuski Azure AD PowerShell. Cmdlet će vratiti jednu od sljedećih vrijednosti:

- **Omogućeno:** omogućena je automatska nadogradnja.

- **Onemogućeno**: automatska je nadogradnja onemogućena.

- **Obustavljeno:** sustav više ne ispunjava uvjete za primanje automatskih nadogradnji. Tu vrijednost ne možete konfigurirati; postavlja ga sustav.

Dodatne informacije potražite u članku [Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Da biste preuzeli najnoviju verziju servisa Azure AD Povezivanje, idite na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
