---
title: Korištenje profila e-pošte s intuneom
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554775"
---
# <a name="using-email-profiles-with-intune"></a>Korištenje profila e-pošte s intuneom

Intune se može koristiti za stvaranje i implementaciju profila e-pošte za izvorni (ugrađeni) klijent e-pošte na više platformi uređaja.

Informacije o nekim ograničenjima povezanima s profilima e-pošte, uključujući način rukovanja prisutnošću postojećih profila i uklanjanje profila [e-pošte, potražite u članku Dodavanje postavki e-pošte uređajima koji koriste Intune](https://docs.microsoft.com/intune/email-settings-configure).

Dodatne informacije o stvaranju profila e-pošte za svaku platformu uređaja potražite u članku:

[Postavke Android uređaja za konfiguriranje e-pošte, provjere autentičnosti i sinkronizacije u aplikaciji Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Dodavanje postavki e-pošte za iOS i iPadOS uređaje u programu Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Postavke profila e-pošte u programu Microsoft Intune za uređaje sa sustavom Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Postavke profila e-pošte za uređaje sa sustavom Windows 10 u programu Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Uobičajeni problem sa sinkronizacijom**

**Knox na Profilu e-pošte androida sprječava sinkronizaciju korisničkih kontakata, kalendara i zadataka s korisničkim uređajima.**

Knox na Android KNOX profilu e-pošte nudi administratoru mogućnost da odluči koje se vrste sadržaja sinkroniziraju s uređajem postavljanjem svakog na omogućeno.

Ako je postavka za bilo koju vrstu sadržaja postavljena na **Nije konfigurirano (zadano),** ta se vrsta sadržaja ne sinkronizira automatski. Korisnik može omogućiti vrstu sadržaja koju žele izravno na uređaju ručno, ali tu konfiguraciju prebriše postavka pravila Intune, a sinkronizacija prestaje s tom vrstom sadržaja.

