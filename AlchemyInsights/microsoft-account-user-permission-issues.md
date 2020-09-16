---
title: Otklanjanje poteškoća s problemom – korisnik nije pronađen u direktoriju
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725399"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Otklanjanje poteškoća s problemom – korisnik nije pronađen u direktoriju

Ako korisnici prime poruku o pogrešci "korisnik se ne može pronaći" u direktoriju, pokušajte ponovno gdje je vrsta problema korisnik koji nije u direktoriju.

Rješavanje problema može se dovršiti u sljedećim koracima.

- Provjerite je li račun koji je prihvatio pozivnicu za e-poštu isti račun koji se koristi za prijavu kasnije. Provjerite koristi li korisnik isti račun za prihvaćanje poziva i prijava na web-mjesto. 

Dodatne informacije potražite u članku [upravljanje pseudonimima za Microsoftov račun </a> za upravljanje prijavom u Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Dođite do svih web-mjesta u kojima korisnik prima pogrešku. 

Na kraj URL-a web-mjesta dodajte "/_layouts/15/People.aspx/membershipgroupid = 0" (unutar dvostrukih navodnika). 

Primjer: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Odaberite korisnika s popisa.

- Na vrpci kliknite **Ukloni korisničke dozvole** . 
-  Dodajte natrag korisnika i ponovno pošaljite pozivnicu korisniku.

