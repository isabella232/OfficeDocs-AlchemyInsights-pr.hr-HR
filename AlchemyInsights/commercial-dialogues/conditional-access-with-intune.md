---
title: Korištenje uvjetnog pristupa uz Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005766"
---
# <a name="using-conditional-access-with-intune"></a>Korištenje uvjetnog pristupa uz Intune

Za korištenje uvjetnog pristupa uz Intune potrebna su tri koraka:

- [Stvorite pravilnik o usklađenosti da biste definirali postavke koje je potrebno posinjeti prije nego što se uređaj smatra usklađenim. Uređaj, primjerice, mora imati pin od najmanje 6 znamenki da bi se smatrao usklađenim.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Stvorite pravilnik uvjetnog pristupa koji definira koji se resursi štite i koje uvjete je potrebno zadostiti da biste pristupili tim resursima. Uređaj, primjerice, mora biti usklađen prije pristupanja poslovnoj e-pošti.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Provjerite jesu li pravila usklađenosti i pravilniki uvjetnog pristupa ciljani na željene grupe korisnika. To može zahtijevati stvaranje određenih grupa korisnika u Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Dodatne informacije...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
