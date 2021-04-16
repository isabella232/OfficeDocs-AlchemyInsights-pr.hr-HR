---
title: Mogućnost otključavanja otiskom prsta u sustavu Windows 10
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
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796669"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Mogućnost otključavanja otiskom prsta u sustavu Windows 10

**Omogućivanje otiska prsta u sustavu Windows Hello**

Da biste otključali Windows 10 pomoću otiska prsta, morate postaviti otisak prsta značajke Windows Hello tako da dodate (ostavljajući sustavu Windows da nauči prepoznati) barem jedan prst. 

1. Otvorite **Postavke > računi > mogućnosti prijave** (ili kliknite [ovdje).](ms-settings:signinoptions?activationSource=GetHelp) Na popisu će biti dostupne mogućnosti prijave. Na primjer:

    ![Mogućnosti prijave.](media/sign-in-options.png)

2. Kliknite ili dodirnite **Otisak prsta značajke Windows Hello**, a zatim **Postavi**. U prozoru za postavljanje značajke Windows Hello **kliknite Početak rada**. Aktivirat će se senzor otiska prsta i od vas će se tražiti da postavite prst na senzor:

   ![Senzor otiska prsta.](media/fingerprint-sensor.png)

3. Slijedite upute koje će od vas tražiti da više puta skenirate prst. Kada to završite, možete dodati i druge prste koje biste mogli koristiti za prijavu. Kada se sljedeći put prijavite u Windows 10, za to ćete imati mogućnost korištenja otiska prsta.

**Windows Hello Fingerprint not available as a sign-in option**

Ako se u mogućnostima prijave ne prikazuje otisak prsta u sustavu Windows Hello **,** to znači da Windows nije upoznat s čitačem otisaka prstiju/skenerom priloženim na PC-ju ili da pravilnik sustava sprječava njegovo korištenje (ako, primjerice, računalom upravlja vaše radno mjesto). Da biste otklonili poteškoće: 

1. Odaberite **gumb Start** na programskoj traci i potražite Upravitelj **uređaja**.

2. Kliknite ili dodirnite da biste **otvorili Upravitelj uređaja**.

3. U upravitelju uređaja proširite Biometrijske uređaje klikom na ševron.

   ![Biometrijski uređaji.](media/biometric-devices.png)

4. Skener otiska prsta trebao bi biti naveden kao biometrijski uređaj, kao što je synaptics WBDI skener:

   ![Biometrijski uređaji.](media/biometric-devices-expanded.png)

5. Ako se skener otiska prsta ne prikazuje, a skener je integriran u PC, idite na web-mjesto proizvođača PC-ja. U odjeljku tehničke podrške za model PC-ja potražite upravljački program za Windows 10 za skener koji možete instalirati.

6. Ako je skener odvojen od PC-ja (priložen putem USB-a), idite na web-mjesto proizvođača skenera da biste pronašli i instalirali softver za upravljačke programe uređaja sa sustavom Windows 10 za model skenera koji imate.
