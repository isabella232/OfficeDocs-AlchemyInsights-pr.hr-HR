---
title: Rješavanje problema - Korisnik nije pronađen u direktoriju
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702730"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Rješavanje problema - Korisnik nije pronađen u direktoriju

Ako korisnik jesu primanje poruka o pogreški " korisnik ne moći' biti postaviti" in imenik, ugoditi probati opet gdje svi Ispostavljati je Korisnik ne in imenik.

Da biste otklonili problem, možete izvršiti sljedeće korake.

- Provjerite je li račun koji je prihvatio pozivnicu za e-poštu isti račun koji se kasnije koristi za prijavu. Provjerite koristi li korisnik isti račun za prihvaćanje pozivnice i prijavu na web-mjesto. 

Dodatne informacije [potražite u odjeljku Upravljanje pseudonimima</a> za Microsoftov račun radi upravljanja prijavom na Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Pronađite svako web-mjesto(e) na kojem korisnik prima pogrešku. 

Dodajte "/_layouts/15/people.aspx/membershipgroupid=0" (unutar dvostrukih navodnika) do kraja URL-a web-mjesta. 

Primjer: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Odaberite korisnika s popisa.

- Na vrpci kliknite **Ukloni korisničke dozvole.** 
-  Dodajte natrag korisnika i ponovno pošaljite pozivnicu korisniku.

