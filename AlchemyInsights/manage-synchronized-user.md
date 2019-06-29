---
title: Upravljanje sinkronizirane korisnika
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380497"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Nije moguće postaviti adresu e-pošte primarnog ili promijeniti korisničke atribute

Ako sinkronizacija imenik omogućen za vaše okruženje neki atributi korisnik ili objekt nije moguće promijeniti pomoću centra za administraciju.
Da biste upravljali potpuno sinkronizirane korisnika i njihove atribute, koristiti vaš aktivni imenik lokalne korisnike i grupe konzole za upravljanje (adsiedit.msc).  

Umjesto toga, možete promijeniti pojedinačni korisnici ili atribute za sinkronizirane korisnici pomoću powershell kao što je prikazano u ove uobičajeni primjeri: 
- Skup MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Skup MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test User" - Prezime "Korisnički"-Naslov "Upravitelja"-odjel "HR"
- Ukloni MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com