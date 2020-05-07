---
title: Exchange PowerShell i osnovna provjera autentičnosti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015681"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell i osnovna provjera autentičnosti

Najnovije informacije o povezivanju sa sustavom Exchange Online PowerShell bez upotrebe osnovne provjere autentičnosti [pronađite ovdje](https://aka.ms/psbasicauth).

Imajte na umu da osnovna provjera autentičnosti još uvijek mora biti omogućena na klijentskom uređaju.
Novi modul PowerShell V2 koristi modernu provjeru autentičnosti kako bi uspostavio vezu i omogućio sve V2 cmdlete koji se oslanjaju na REST. Osim V2 cmdleta, on vam omogućuje i pristup starijim cmdletima za Remote PowerShell (RPS) za koje je potrebno uspostaviti sesiju ljuske Remote PowerShell. Uspostavljanje RPS sesije na računalu sa sustavom Windows zahtijeva da se na klijentskom računalu omogući WinRM BasicAuth čak i u slučaju da za provjeru autentičnosti prilikom pristupanja servisu modul koristi mehanizam moderne provjere autentičnosti. Za prijenos tokena moderne provjere autentičnosti koristi se komunikacijski kanal provjere autentičnosti WinRM Basic. Ako je provjera autentičnosti WinRM Basic onemogućena na klijentskom računalu, novi će V2 cmdleti i dalje funkcionirati (no stariji RPS cmdleti neće).
