---
title: Promijenite adresu e-pošte grupe sustava Microsoft 365 ili aplikacije Microsoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995614"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Promijenite adresu e-pošte grupe sustava Microsoft 365 ili aplikacije Microsoft Teams

Možete promijeniti adresu e-pošte grupe sustava Microsoft 365 ili aplikacije Microsoft Teams uz pomoć [Centra za administratore okruženja Microsoft 365](https://admin.microsoft.com/). Samo odaberite grupu i @uredite adresu e-pošte.

Možete upotrijebiti i sljedeću naredbu EXO PowerShell za promjenu primarne SMTP adrese grupe sustava Microsoft 365/aplikacije Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Primjer:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
