---
title: Rješavanje problema-korisnik nije pronađen u direktoriju
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768793"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Rješavanje problema-korisnik nije pronađen u direktoriju

Ako korisnici primaju poruku o pogrešci "korisnik ne može naći" u direktoriju, pokušajte ponovno gdje vrsta problema je korisnik nije u direktoriju.

Za otklanjanje problema možete dovršiti sljedeće korake.

- Provjerite je li račun koji je prihvatio pozivnicu e-poštom isti račun koji se koristi za prijavu kasnije. Provjerite koristi li korisnik isti račun za prihvaćanje pozivnice i prijavu na web-mjesto. 

Dodatne informacije potražite u članku [kako upravljati pseudonime za Microsoftov račun</a> za upravljanje uredom 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Pregledajte Svaka web-mjesta u kojima korisnik prima pogrešku. 

Dodajte "/_layouts/15/. aspx/membershipgroupid = 0" (unutar dvostrukih navodnika) do kraja URL-a web-mjesta. 

Primjer: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Odaberite korisnika s popisa.

- Kliknite **Ukloni korisničke dozvole** s vrpce. 
-  Dodajte korisnika natrag i ponovno pošaljite pozivnicu korisniku.

