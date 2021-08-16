---
title: Uvjetni pristup uz Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069704"
---
# <a name="conditional-access-with-intune"></a>Uvjetni pristup uz Intune

Za  **korištenje uvjetnog pristupa**  uz Intune potrebna su tri koraka:

- Stvorite pravilnik **o usklađenosti** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios) [, Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) da biste definirali postavke koje je potrebno zadeti prije nego što se uređaj smatra usklađenim. Uređaj, primjerice, mora imati pin od najmanje 6 znamenki da bi se smatrao usklađenim.
- Stvorite pravilnik **uvjetnog pristupa**  koji definira koji se resursi štite i koje uvjete je potrebno zadostiti da biste pristupili tim resursima.  [Uređaj, primjerice,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  mora biti usklađen prije pristupanja poslovnoj e-pošti.
- Provjerite jesu **li pravila usklađenosti**  **i pravilniki**  uvjetnog pristupa ciljani na željene grupe korisnika. To može zahtijevati stvaranje određenih grupa korisnika u Azure Active Directory.

**Korisne veze:**

[Pregled usklađenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)

[Otklanjanje poteškoća s ca](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Pravilnik o otklanjanju poteškoća](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Da biste zaštitili e-poštu (Exchange na mreži) od pristupa putem uređaja koji nisu kompatibilni, moraju se slijediti oba dokumenta:

1. [Zaštita pristupa e-pošti s uređaja pomoću EAS-a](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Zaštita pristupa e-pošti s uređaja pomoću modernih klijenata za provjeru autentičnosti kao što su Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)