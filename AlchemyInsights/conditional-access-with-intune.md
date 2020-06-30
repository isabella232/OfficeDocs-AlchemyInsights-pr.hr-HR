---
title: Uvjetni pristup s intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931422"
---
# <a name="conditional-access-with-intune"></a>Uvjetni pristup s intune

Korištenje **uvjetnog pristupa** s intune zahtijeva 3 koraka:

- Stvorite **pravila usklađenosti** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) da biste definirali postavke koje se moraju ispuniti prije nego što se uređaj smatra sukladnim. Na primjer, uređaj mora imati pribadaču od najmanje 6 znamenki prije nego što se smatra sukladnim.
- Stvorite **pravilo uvjetnog pristupa** koje definira koji su resursi zaštićeni i koji uvjeti moraju biti ispunjeni za pristup tim resursima.  [Na primjer,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) uređaj mora biti sukladan prije pristupanja korporativnoj e-pošti.
- Provjerite jesu li **pravila usklađenosti** i **pravila uvjetnog pristupa** usmjerena na željene grupe korisnika. To može zahtijevati stvaranje određenih grupa korisnika u servisu Azure Active Directory.

**Korisni linkovi:**

[Pregled usklađenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)

[Rješavanje problema CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Pravila za otklanjanje poteškoća](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Da biste e-poštu (Exchange online) zaštitili od pristupa neusklađenih uređaja, oba dokumenta moraju se slijediti:

1. [Zaštita pristupa e-pošti s uređaja pomoću EAS-a](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Zaštita pristupa e-pošti s uređaja pomoću modernih klijenata za provjeru autentičnosti kao što je Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)