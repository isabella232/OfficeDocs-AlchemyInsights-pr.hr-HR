---
title: Otklanjanje poteškoća – korisnik nije pronađen u direktoriju
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098162"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Otklanjanje poteškoća – korisnik nije pronađen u direktoriju

Ako korisnici primaju poruku o pogrešci "korisnik nije moguće pronaći" u direktoriju, pokušajte ponovno kada vrsta problema nije korisnik u direktoriju.

Da biste riješili problem, možete dovršiti sljedeće korake.

- Provjerite je li račun koji je prihvatio pozivnicu za e-poštu isti račun koji se koristi za kasnije prijavu. Provjerite koristi li korisnik isti račun da bi prihvatio pozivnicu i prijavio se na web-mjesto. 

Dodatne informacije potražite u članku Upravljanje pseudonimima za Microsoftov račun radi upravljanja Microsoft 365 [ </a> prijavom](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Pronađite svako web-mjesto na kojem korisnik prima pogrešku. 

Dodajte "/_layouts/15/people.aspx/membershipgroupid=0" (unutar dvostrukih navodnike) na kraj URL-a web-mjesta. 

Primjer: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Na popisu odaberite korisnika.

- Kliknite **Ukloni korisničke dozvole** s vrpce. 
-  Dodajte korisnika i ponovno ga dodajte korisniku.

