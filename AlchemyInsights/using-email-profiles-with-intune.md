---
title: Korištenje profila e-pošte pomoću aplikacije Intune
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
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919415"
---
# <a name="using-email-profiles-with-intune"></a>Korištenje profila e-pošte pomoću aplikacije Intune

Intune se može koristiti za stvaranje i implementaciju profila e-pošte za nativni (ugrađeni) klijent e-pošte na više platformi uređaja.

Informacije o nekim ograničenjima povezanima s profilima e-pošte, uključujući način obrade prisutnosti postojećih profila i uklanjanje profila e-pošte potražite u članku Dodavanje postavki e-pošte na uređaje [koji koriste Intune](https://docs.microsoft.com/intune/email-settings-configure).

Dodatne informacije o stvaranju profila e-pošte za svaku platformu uređaja potražite u članku:

[Postavke uređaja sa sustavom Android za konfiguriranje e-pošte, provjere autentičnosti i sinkronizacije u aplikaciji Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Dodavanje postavki e-pošte za uređaje sa sustavom iOS i iPadOS u Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Postavke profila e-pošte u Microsoft Intune za uređaje sa sustavom Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Postavke profila e-pošte za uređaje sa Windows 10 u Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Uobičajeni problem sa sinkronizacijom**

**KNOX na profilu e-pošte sustava Android korisnicima onemoguće sinkronizaciju kontakata, kalendara i zadataka s korisničkim uređajima.**

KNOX na profilu e-pošte sustava Android KNOX administratoru nudi mogućnost odlučivanja koje će se vrste sadržaja sinkronizirati s uređajem tako da ih postavite na omogućeno.

Ako je postavka za neku od vrsta sadržaja postavljena na **Nije konfigurirano** (zadano), ta se vrsta sadržaja ne sinkronizira automatski. Korisnik može ručno omogućiti vrstu sadržaja koju želi izravno na uređaju, ali tu konfiguraciju prebriše postavka pravilnika intune, a sinkronizacija se zaustavlja za tu vrstu sadržaja.

