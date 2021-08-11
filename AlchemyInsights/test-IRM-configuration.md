---
title: Testiranje konfiguracije IRM-a za nove mogućnosti OME-a
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812430"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Testiranje konfiguracije IRM-a za nove mogućnosti OME-a

Da biste provjerili je Microsoft 365 klijent konfiguriran za korištenje novih mogućnosti OME-a, pokrenite sljedeće cmdlete dok ste [povezani s Exchange Online PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Provjerite konfiguraciju IRM-a klijenta pokretanjem `Get-IRMConfiguration` . Provjerite jesu li te vrijednosti postavljene na **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Pomoću domene, adrese pošiljatelja i primatelja pokrenite `Test-IRMConfiguration` . Ako test ne prođe, istražite konfiguraciju IRM-a.

Dodatne informacije o provjeri konfiguracije IRM-a potražite u članku Provjera nove [konfiguracije OME-a u Exchange Online PowerShell](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).