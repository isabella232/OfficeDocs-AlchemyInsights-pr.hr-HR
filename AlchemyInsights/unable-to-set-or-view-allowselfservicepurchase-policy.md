---
title: Nije moguće postaviti ili prikazati pravilo Allowselfservicekupnja
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735191"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nije moguće postaviti ili prikazati pravilo Allowselfservicekupnja

Kada pokušate postaviti ili prikazati pravilo Allowselfservicekupnja, prikazat će vam se sljedeća poruka o pogrešci:

*Funkcija HandleError: nije uspjelo dohvaćanje pravilnika o proizvodu s PolicyId ' Allowselfservicekupnja ', ErrorMessage-osnovna veza je zatvorena: došlo je do neočekivane pogreške na slanju.*

To može biti zbog starije verzije sigurnosnog sloja za transport (TLS). Da biste povezali servis MSCommerce, morate koristiti TLS 1,2 ili noviji.  

Pokušajte poduzeti sljedeće korake da biste omogućili/postavili TLS protokol na 1,2, potvrdili i pokušali ponovno.
 1. U naredbeni upit za PowerShell (PS C: \) Unesite sljedeću naredbu da biste postavili TLS protokol na verziju 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Potvrđivanje TLS protokola (s) u upotrebi, uz sljedeću naredbu:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Ponovno pokušajte izvršiti naredbe Dohvati ili Ažuriraj po potrebi.

