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
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114761"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nije moguće postaviti primarnu adresu e-pošte, promijeniti korisničke atribute ili ukloniti/izbrisati sinkroniziranog korisnika

Ako je sinkronizacija direktorija omogućena za vaše okruženje, neke atribute korisnika ili objekta nije moguće promijeniti pomoću Centar za administratore okruženja Microsoft 365.

Da biste u potpunosti upravljali sinkroniziranim korisnicima i svim njihovim atributima, koristite lokalnu konzolu za upravljanje active directory i grupama (adsiedit.msc).  

Možete i promijeniti pojedinačne korisnike ili atribute za sinkronizirane korisnike pomoću ljuske powershell, kao što je prikazano u ovim uobičajenim primjerima:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
