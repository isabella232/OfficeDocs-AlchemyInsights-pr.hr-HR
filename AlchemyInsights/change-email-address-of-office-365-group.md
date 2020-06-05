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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580649"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Promjena adrese e-pošte grupe sustava Microsoft 365

Adresu e-pošte grupe microsoft 365 možete promijeniti pomoću centra za administratore. Samo odaberite grupu i odaberite @edit adresu e-pošte.

Možete koristiti i sljedeću naredbu EXO PowerShell da biste promijenili primarnu SMTP adresu grupe microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Primjer:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
