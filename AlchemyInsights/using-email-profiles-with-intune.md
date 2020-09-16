---
title: Korištenje profila e-pošte s dodatkom Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653280"
---
# <a name="using-email-profiles-with-intune"></a>Korištenje profila e-pošte s dodatkom Intune

Intune se može koristiti za stvaranje i implementaciju profila e-pošte za urođenik (ugrađeno) klijenta e-pošte na više platformi uređaja.

Informacije o nekim od ograničenja povezanih s profilima e-pošte, uključujući način na koji se obrađuju prisutnost postojećih profila i kako ukloniti profile e-pošte potražite [u članku Dodavanje postavki e-pošte na uređaje pomoću aplikacije Intune](https://docs.microsoft.com/intune/email-settings-configure).

Dodatne informacije o stvaranju profila e-pošte za svaku platformu uređaja potražite u članku:

[Postavke uređaja sa sustavom Android za konfiguriranje e-pošte, provjere autentičnosti i sinkronizacije u programu Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Dodavanje postavki e-pošte za iOS i iPadOS uređaje u programu Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Postavke profila e-pošte u aplikaciji Microsoft Intune za uređaje sa sustavom Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Postavke profila za e-poštu za uređaje sa sustavom Windows 10 u programu Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Zajednički problem s sinkronizacijom**

**KNOX na servisu Android profile za e-poštu onemogućuje sinkronizaciju korisnika, kalendara i zadataka s korisničkim uređajima.**

KNOX na Android KNOX profilu e-pošte nudi administratore mogućnost odluke o tome koje se vrste sadržaja sinkroniziraju s uređajem tako da se svaki od njih omogući.

Ako je postavka za neku vrstu sadržaja postavljena na **nekonfiguriranu** (zadano), ta se vrsta sadržaja ne sinkronizira automatski. Korisnik može omogućiti ručno umetanje vrste sadržaja na uređaj, ali ta je konfiguracija prebrijela postavku pravilnika Intune, a sinkronizacija prestaje za tu vrstu sadržaja.

