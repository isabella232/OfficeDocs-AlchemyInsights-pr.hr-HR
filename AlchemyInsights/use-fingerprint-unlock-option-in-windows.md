---
title: Mogućnost otključavanja otiskom prsta u Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971879"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Mogućnost otključavanja otiskom prsta u Windows 10

**Omogućivanje Windows Hello otiska prsta**

Da biste Windows 10 pomoću otiska prsta, morate postaviti otisak prsta Windows Hello tako da dodate (Windows naučite prepoznati) barem jednim prstom. 

1. Idite **na Postavke > računi > mogućnosti prijave** (ili kliknite [ovdje).](ms-settings:signinoptions?activationSource=GetHelp) Na popisu će biti dostupne mogućnosti prijave. Na primjer:

    ![Mogućnosti prijave.](media/sign-in-options.png)

2. Kliknite ili dodirnite **Windows Hello otisak prsta**, a zatim **Postavi**. U prozoru Windows Hello postavljanje kliknite **Početak rada**. Aktivirat će se senzor otiska prsta i od vas će se tražiti da postavite prst na senzor:

   ![Senzor otiska prsta.](media/fingerprint-sensor.png)

3. Slijedite upute koje će od vas tražiti da više puta skenirate prst. Kada to završite, možete dodati i druge prste koje biste mogli koristiti za prijavu. Kada se sljedeći put Windows 10, za to ćete imati mogućnost korištenja otiska prsta.

**Windows Hello Otisak prsta nije dostupan kao mogućnost prijave**

Ako Windows Hello otisak prsta nije prikazan kao mogućnost u mogućnostima prijave, to znači da Windows nije upoznat s čitačem otisaka prstiju/skenerom priloženim NA **PC-ju** ili da pravilnik sustava sprječava njegovo korištenje (ako, primjerice, vašim PC-jem upravlja vaše radno mjesto). Da biste otklonili poteškoće: 

1. Odaberite **gumb Start** na programskoj traci i potražite Upravitelj **uređaja**.

2. Kliknite ili dodirnite da biste **otvorili Upravitelj uređaja**.

3. U upravitelju uređaja proširite Biometrijske uređaje klikom na ševron.

   ![Biometrijski uređaji.](media/biometric-devices.png)

4. Skener otiska prsta trebao bi biti naveden kao biometrijski uređaj, kao što je synaptics WBDI skener:

   ![Biometrijski uređaji.](media/biometric-devices-expanded.png)

5. Ako se skener otiska prsta ne prikazuje, a skener je integriran u PC, idite na web-mjesto proizvođača PC-ja. U odjeljku tehničke podrške za model PC-ja potražite Windows 10 upravljački program za skener koji možete instalirati.

6. Ako je skener odvojen od PC-ja (priložen putem USB-a), idite na web-mjesto proizvođača skenera da biste pronašli i instalirali Windows 10 upravljački program uređaja za model skenera koji imate.
