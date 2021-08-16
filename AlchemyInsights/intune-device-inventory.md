---
title: Intune Device Inventory
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014064"
---
# <a name="intune-device-inventory"></a>Intune Device Inventory

Oštrica Uređaji omogućuje administratorski uvid u uređaje u upravljanju u programu Intune na temelju uređaja. Prikazani podaci obuhvaćaju: hardver, otkrivene aplikacije, stanje usklađenosti uređaja i stanje konfiguracije uređaja.

Podaci inventara za hardver i otkrivene aplikacije prikupljaju se u sedmodnevni ciklus. Aplikacije i određeni elementi prijavljenog hardvera razlikuju se ovisno o operacijskom sustavu uređaja i o tome je li uređaj u osobnom ili korporativnom vlasništvu.

Dodatne informacije potražite u [odjeljku Pojedinosti o uređaju u programu Intune](https://docs.microsoft.com/intune/device-inventory).

**Najčešća pitanja**

P: Ne primam potpuni popis inventara aplikacija koje se nalaze na uređajima Windows intune. zašto ne?

O: U ovom su trenutku navedene samo moderne aplikacije za Windows 10 pc-jeve koji su identificirani kao korporativni uređaji. Intune ne prikuplja podatke o aplikacijama sustava Win32 instaliranima na tim uređajima.

P: Zašto se telefonski brojevi ne prikupljaju sa svih uređaja?

O: Telefoni kategorizirani kao korporativni uređaji u aplikaciji Intune ne identificiraju se s punim telefonskim brojem kada, primjerice, pokrenete izvješće o inventaru mobilnog uređaja. Telefonski brojevi za ponijeti na vlastiti uređaj uvijek su djelomično maskirani zvjezdicama (****) i prikazuju samo zadnje četiri znamenke.