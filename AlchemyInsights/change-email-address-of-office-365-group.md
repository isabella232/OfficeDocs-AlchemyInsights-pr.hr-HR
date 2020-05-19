---
title: Promjena adrese e-pošte grupe sustava Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282613"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Promjena adrese e-pošte grupe sustava Microsoft 365

Adresu e-pošte grupe microsoft 365 možete promijeniti pomoću centra za administratore. Samo odaberite grupu i odaberite @edit adresu e-pošte.

Možete koristiti i naredbu EXO PowerShell da biste promijenili primarnu SMTP adresu grupe sustava Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Primjer:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
