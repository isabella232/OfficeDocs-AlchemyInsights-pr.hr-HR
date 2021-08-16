---
title: Exchange PowerShell i osnovna provjera autentičnosti
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069236"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell i osnovna provjera autentičnosti

Najnovije informacije o povezivanju sa sustavom Exchange Online PowerShell bez upotrebe osnovne provjere autentičnosti [pronađite ovdje](https://aka.ms/exops-docs). Modul PowerShell V2 ne upotrebljava osnovnu provjeru autentičnosti.

Imajte na umu da osnovna provjera autentičnosti još uvijek mora biti omogućena na klijentskom uređaju.
Novi modul PowerShell V2 koristi modernu provjeru autentičnosti kako bi uspostavio vezu i omogućio sve V2 cmdlete koji se oslanjaju na REST. Osim V2 cmdleta, on vam omogućuje i pristup starijim cmdletima za Remote PowerShell (RPS) za koje je potrebno uspostaviti sesiju ljuske Remote PowerShell. Uspostavljanje RPS sesije na računalu sa sustavom Windows zahtijeva da se na klijentskom računalu omogući WinRM BasicAuth čak i u slučaju da za provjeru autentičnosti prilikom pristupanja servisu modul koristi mehanizam moderne provjere autentičnosti. Za prijenos tokena moderne provjere autentičnosti koristi se komunikacijski kanal provjere autentičnosti WinRM Basic. Ako je provjera autentičnosti WinRM Basic onemogućena na klijentskom računalu, novi će V2 cmdleti i dalje funkcionirati (no stariji RPS cmdleti neće).
