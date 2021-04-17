---
title: Upravljanje sinkroniziranim korisnikom
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823959"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nije moguće postaviti primarnu adresu e-pošte, promijeniti korisničke atribute ili ukloniti/izbrisati sinkroniziranog korisnika

Ako je sinkronizacija direktorija omogućena za vaše okruženje, neke atribute korisnika ili objekta nije moguće promijeniti pomoću centra za administratore sustava Microsoft 365.

Da biste u potpunosti upravljali sinkroniziranim korisnicima i svim njihovim atributima, koristite lokalnu konzolu za upravljanje active directory i grupama (adsiedit.msc).  

Možete i promijeniti pojedinačne korisnike ili atribute za sinkronizirane korisnike pomoću ljuske powershell, kao što je prikazano u ovim uobičajenim primjerima:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
