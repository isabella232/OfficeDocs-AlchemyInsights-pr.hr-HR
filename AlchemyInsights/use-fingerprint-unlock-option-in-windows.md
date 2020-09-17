---
title: Korištenje mogućnosti otključavanja otisaka prstiju u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795236"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Korištenje mogućnosti otključavanja otisaka prstiju u sustavu Windows 10

**Omogućivanje otiska prsta u sustavu Windows Hello**

Da biste otključali Windows 10 pomoću otiska prsta, morate postaviti otisak prsta u sustavu Windows Hello dodavanjem (ostavljajući Windows da sazna da prepozna) barem jedan prst. 

1. Idite na **postavke > računi > mogućnosti prijave** (ili kliknite [ovdje](ms-settings:signinoptions?activationSource=GetHelp)). Dostupne mogućnosti prijave prikazat će se na popisu. Na primjer:

    ![Mogućnosti prijave](media/sign-in-options.png)

2. Kliknite ili dodirnite **otisak prsta u sustavu Windows Hello**, a zatim kliknite **Postavi**. U prozoru Postavljanje sustava Windows Hello kliknite **početak rada**. Senzor otiska prsta aktivirat će se i od vas će se zatražiti da postavite prst na senzor:

   ![Senzor otisaka prstiju.](media/fingerprint-sensor.png)

3. Slijedite upute koje će vas upitati da opetovano skenirate prst. Kada ovo završite, imat ćete mogućnost dodavanja drugih prstiju koje želite koristiti za prijavu. Kada se sljedeći put prijavite u Windows 10, imat ćete mogućnost korištenja otiska prsta da biste to učinili.

**Otisak prsta u sustavu Windows Hello nije dostupan kao mogućnost prijave**

Ako se otisci zaslona u sustavu Windows Hello ne prikazuju kao mogućnost u **mogućnostima prijave**, znači da Windows nije svjestan bilo kojeg čitača otisaka prstiju koji je priključen na PC ili da pravilnik sustava sprječava njegovo korištenje (ako na PC-ju upravlja vaše radno mjesto). Otklanjanje poteškoća: 

1. Odaberite gumb **Start** na programskoj traci i potražite **upravitelja uređaja**.

2. Kliknite ili dodirnite da biste otvorili **Upravitelj uređaja**.

3. U upravitelju uređaja proširite Biometrijski uređaji tako da kliknete njegov Chevron.

   ![Biometrijskih uređaja.](media/biometric-devices.png)

4. Skener otisaka prstiju trebao bi biti naveden kao biometrijski uređaj, kao što je sinaptički WBDI Scanner:

   ![Biometrijskih uređaja.](media/biometric-devices-expanded.png)

5. Ako vam se ne prikaže skener otisaka prstiju, a skener je integriran na PC, otvorite web-mjesto proizvođača PC-ja. U odjeljku tehnička podrška za PC model potražite upravljački program za Windows 10 za skener koji možete instalirati.

6. Ako je skener odvojen od PC-ja (priključen putem USB-a), otvorite web-mjesto proizvođača skenera da biste pronašli i instalirali upravljački program za uređaj sa sustavom Windows 10 za model skenera koji imate.
