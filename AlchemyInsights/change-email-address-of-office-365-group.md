---
title: Promjena adrese e-pošte grupe sustava Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819036"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Promjena adrese e-pošte grupe sustava Microsoft 365

Adresu e-pošte grupe sustava Microsoft 365 možete promijeniti pomoću centra za administratore. Samo odaberite grupu i @uredite adresu e-pošte.

Pomoću naredbe EXO PowerShell možete promijeniti i primarnu SMTP adresu grupe microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Primjer:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
