---
title: 932 Nadogradnja AADConnect-a
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806031"
---
# <a name="upgrade-azure-ad-connect"></a>Nadogradnja servisa Azure AD Connect

Po zadanom je omogućena automatska nadogradnja za Azure AD Connect, čime se omogućuje da koristite najnoviju verziju. Da biste potvrdili postavke automatskog nadogradnje, upotrijebite cmdlet **Get-Adsyncautouprazreda** u aplikaciji Azure ad PowerShell. Cmdlet će vratiti jednu od sljedećih vrijednosti:

- **Omogućeno**: omogućeno je automatsko ažuriranje.

- **Onemogućeno**: automatska nadogradnja je onemogućena.

- **Suspendirane**: sustav više ne ispunjava uvjete za primanje automatskih nadogradnji. Ne možete konfigurirati tu vrijednost; postavlja ga sustav.

Dodatne informacije potražite u članku [Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Da biste preuzeli najnoviju verziju servisa Azure AD Connect, otvorite [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
