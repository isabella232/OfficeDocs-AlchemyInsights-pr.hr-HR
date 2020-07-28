---
title: Intune inventar uređaja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438914"
---
# <a name="intune-device-inventory"></a>Intune inventar uređaja

Oštrica Uređaji pruža administratorski uvid u uređaje pod upravljanjem u intuneu po uređaju. Prikazane informacije uključuju: Hardver, Otkrivene aplikacije, Stanje usklađenosti uređaja i stanje konfiguracije uređaja.

Podaci o inventaru za hardver i otkrivene aplikacije prikupljaju se sedmodnevnim ciklusom. Aplikacije i specifični elementi hardvera koji se prijavljuju razlikuju se ovisno o operacijskom sustavu uređaja i je li uređaj osobno ili u vlasništvu tvrtke.

Dodatne informacije [potražite u odjeljku Prikaz pojedinosti o uređaju u odjeljku Intune](https://docs.microsoft.com/intune/device-inventory).

**Najčešća pitanja**

P: Ne primam potpuni popis inventara aplikacija prisutnih na uređajima windows koji su upisani intune. Zašto ne?

O: Trenutno su navedene samo moderne aplikacije za PC-jeve sa sustavom Windows 10 koji su identificirani kao korporativni uređaji. Intune ne prikuplja informacije o Win32 aplikacijama instaliranima na tim uređajima.

P: Zašto se telefonski brojevi ne prikupljaju sa svih uređaja?

O: Telefoni kategorizirani kao korporativni uređaji u tvrtki Intune ne identificiraju se s punim telefonskim brojem kada, na primjer, pokrenete izvješće o inventaru mobilnih uređaja. Bring-you-vlastiti uređaj telefonski brojevi su uvijek djelomično maskirani sa zvjezdicama (****), i pokazati samo posljednje četiri znamenke.