---
title: Upravljanje sinkroniziranim korisnikom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451392"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nemogućnost postavljanja primarne adrese e-pošte, promjena korisničkih atributa ili uklanjanje/brisanje sinkroniziranog korisnika

Ako je za vašu okolinu omogućena sinkronizacija direktorija, neki korisnici ili atributi objekta ne mogu se promijeniti pomoću centra za administratore sustava Microsoft 365.

Da biste u potpunosti upravljali sinkroniziranim korisnicima i svim njihovim atributima, koristite lokalne korisnike servisa Active Directory i konzolu za upravljanje grupama (Adsiedit. msc).  

Alternativno, možete promijeniti pojedinačne korisnike ili atribute za sinkronizirane korisnike pomoću komponente PowerShell, kao što je prikazano u ovim uobičajenim primjerima:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
