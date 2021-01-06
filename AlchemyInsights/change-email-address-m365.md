---
title: Promijenite adresu e-pošte grupe sustava Microsoft 365 ili aplikacije Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756549"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Promijenite adresu e-pošte grupe sustava Microsoft 365 ili aplikacije Microsoft Teams

Možete promijeniti adresu e-pošte grupe sustava Microsoft 365 ili aplikacije Microsoft Teams uz pomoć [Centra za administratore okruženja Microsoft 365](https://admin.microsoft.com/). Samo odaberite grupu i @uredite adresu e-pošte.

Možete upotrijebiti i sljedeću naredbu EXO PowerShell za promjenu primarne SMTP adrese grupe sustava Microsoft 365/aplikacije Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Primjer:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
