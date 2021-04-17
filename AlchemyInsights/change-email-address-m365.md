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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819072"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Promijenite adresu e-pošte grupe sustava Microsoft 365 ili aplikacije Microsoft Teams

Možete promijeniti adresu e-pošte grupe sustava Microsoft 365 ili aplikacije Microsoft Teams uz pomoć [Centra za administratore okruženja Microsoft 365](https://admin.microsoft.com/). Samo odaberite grupu i @uredite adresu e-pošte.

Možete upotrijebiti i sljedeću naredbu EXO PowerShell za promjenu primarne SMTP adrese grupe sustava Microsoft 365/aplikacije Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Primjer:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
