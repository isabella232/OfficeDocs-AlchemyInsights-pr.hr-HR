---
title: Korištenje mogućnosti otključavanja otiska prsta u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588308"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Korištenje mogućnosti otključavanja otiska prsta u sustavu Windows 10

**Omogući otisak prsta za pozdrave u sustavu Windows**

Da biste otključali Windows 10 pomoću otiska prsta, otisak prsta za Pozdrav sustavom Windows morate postaviti tako da dodate (omogućujući sustavu Windows da nauči prepoznati) barem jedan prst. 

1. Idite na **Postavke > Računi > Mogućnosti prijave** (ili kliknite [ovdje](ms-settings:signinoptions?activationSource=GetHelp)). Bit će navedene dostupne mogućnosti prijave. Na primjer:

    ![Opcije prijave.](media/sign-in-options.png)

2. Kliknite ili dodirnite **Otisak prsta za Pozdrav u sustavu Windows**, a zatim **Postavi**. U prozoru za postavljanje značajke Windows Hello kliknite **Početak rada**. Senzor otiska prsta će se aktivirati, a vi ćete biti zatraženo da stavite prst na senzor:

   ![Senzor otiska prsta.](media/fingerprint-sensor.png)

3. Slijedite upute koje će od vas zatražiti da više puta skenirate prst. Kada se to završi, moći ćete dodati druge prste koje biste mogli koristiti za prijavu. Sljedeći put kada se prijavite u Windows 10, imat ćete mogućnost korištenja otiska prsta da biste to učinili.

**Otisak prsta za Pozdrav u sustavu Windows nije dostupan kao mogućnost prijave**

Ako se otisak prsta za Pozdrav u sustavu Windows ne prikazuje kao mogućnost u **mogućnostima prijave,** to znači da Windows nije svjestan čitača otisaka prstiju/skenera priključenog na PC ili da pravilo sustava sprječava njegovo korištenje (ako vašim PC-jem upravlja vaše radno mjesto). Da biste otklonili poteškoće: 

1. Odaberite gumb **Start** na programskoj traci i potražite **Upravitelj uređaja**.

2. Klikom ili dodirom otvorite **Upravitelj uređaja**.

3. U upravitelju uređaja proširite biometrijske uređaje klikom na njegov ševron.

   ![Biometrijski uređaji.](media/biometric-devices.png)

4. Skener otiska prsta trebao bi biti naveden kao biometrijski uređaj, kao što je Synaptics WBDI skener:

   ![Biometrijski uređaji.](media/biometric-devices-expanded.png)

5. Ako se skener otiska prsta ne prikaže, a skener je integriran u PC, posjetite web-mjesto proizvođača PC-ja. U odjeljku tehničke podrške za model PC-ja potražite upravljački program za Windows 10 za skener koji možete instalirati.

6. Ako je skener odvojen od PC-ja (priključenog putem USB-a), posjetite web-mjesto proizvođača skenera da biste pronašli i instalirali upravljački program za upravljački program uređaja sustava Windows 10 za model skenera koji imate.
