---
title: Unos zaliha uređaja
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
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667870"
---
# <a name="intune-device-inventory"></a>Unos zaliha uređaja

Oštrica uređaja sadrži administrator uvid u uređaje u odjeljku Upravljanje u programu Intune na temelju uređaja po uređaju. Prikazane informacije obuhvaćaju: hardver, otkrivene aplikacije, stanje usklađenosti uređaja i stanje konfiguracije uređaja.

Podaci o zalihama za hardver i otkrivene aplikacije prikupljaju se sedmodnevnim ciklusom. Aplikacije i posebni elementi hardvera koji su prijavljeni razlikuju se ovisno o operacijskom sustavu uređaja te je li uređaj osobno ili korporacijski vlasnik.

Dodatne informacije potražite u članku [Prikaz detalja o uređaju u programu Intune](https://docs.microsoft.com/intune/device-inventory).

**Najčešća pitanja**

P: ne primam cijeli popis zaliha aplikacija prisutnih na Intune-upisanih uređaja sa sustavom Windows. zašto ne?

O: u ovom trenutku navedene su samo moderne aplikacije za PC-jeve sa sustavom Windows 10 koje se identificiraju kao korporativni uređaji. Intune ne prikuplja informacije o aplikacijama Win32 koje su instalirane na ovim uređajima.

P: Zašto se brojevi telefonskih brojeva ne prikupljaju na svim uređajima?

A: telefoni kategorizirani kao korporativni uređaji u programu Intune ne identificiraju se s punim telefonskim brojem kada, na primjer, pokrenete izvješće o zalihama mobilnog uređaja. Telefonski brojevi koji donose vlastite uređaje uvijek su djelomično maskirani sa zvjezdicama (* * * *) i prikazuju samo posljednje četiri znamenke.