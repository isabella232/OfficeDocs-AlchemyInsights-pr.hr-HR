---
title: Korištenje uvjetnog pristupa pomoću aplikacije Intune
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
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692696"
---
# <a name="using-conditional-access-with-intune"></a>Korištenje uvjetnog pristupa pomoću aplikacije Intune

Korištenje uvjetnog pristupa pomoću aplikacije Intune zahtijeva tri koraka:

- [Stvaranje pravilnika o usklađenosti za definiranje postavki koje je potrebno ispuniti prije nego što se uređaj smatra sukladnim. Na primjer, uređaj mora imati PIN od najmanje 6 znamenki prije nego što se smatra sukladnim.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Stvorite pravilnik o uvjetnom pristupu koji definira resurse zaštićene i koje uvjete morate ispuniti da biste pristupili tim resursima. Na primjer, uređaj mora biti usklađen prije pristupanja korporativnom e-pošti.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Provjerite jesu li pravila usklađivanja i pravila uvjetnog pristupa usmjerena na željene grupe korisnika. To može zahtijevati stvaranje određenih grupa korisnika u servisu Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Dodatne informacije...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
