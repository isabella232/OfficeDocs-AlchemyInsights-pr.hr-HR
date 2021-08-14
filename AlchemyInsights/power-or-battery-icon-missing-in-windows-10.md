---
title: U sustavu Windows 10 nema ikone napajanja ili baterije
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 82d41844de1eafdf7e0cc38f91416f3b71868e3d5d1b3eb8be0f10abd701ddc8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973299"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>U sustavu Windows 10 nema ikone napajanja ili baterije

Ako uređaj sa sustavom Windows 10 ima bateriju (npr. prijenosno računalo, tablet ili PC povezan s UPS-om putem USB-a), obično se na programskoj traci u blizini sata prikazuje ikona napajanja/baterije, na primjer:

![Ikona baterije](media/battery-icon.png)

Ako ne vidite tu ikonu, možda je skrivena:

1. Otvorite **[Postavke > Personalizacija > Programska traka](ms-settings:taskbar?activationSource=GetHelp)**.

2. U području obavijesti kliknite mogućnost **Odaberite koje će se ikone prikazivati na programskoj traci**.

3. Potom na popisu pronađite stavku **Napajanje** i prebacite njezinu postavku na **Uključeno**.

    ![Prikaži ikonu napajanja na programskoj traci](media/power-icon-on.png)

**Otklanjanje poteškoća**

Ako ste slijedili navedene upute, ali je prekidač **Napajanje** zasivljen ili nije vidljiv, u okvir za pretraživanje na programskoj traci upišite **upravitelj uređaja**, a zatim na popisu rezultata odaberite **Upravitelj uređaja**. U odjeljku **Baterije**, desnom tipkom miša kliknite bateriju svojeg uređaja te kliknite **Onemogući**, a zatim **Da**. Pričekajte nekoliko sekundi pa desnom tipkom miša kliknite bateriju, a zatim **Omogući**. Potom ponovno pokrenite uređaj.

Ako ste slijedili navedene upute, ali se ikona baterije ne prikazuje na programskoj traci, u okvir za pretraživanje na programskoj traci upišite **upravitelj zadataka**, a zatim na popisu rezultata kliknite **Upravitelj zadataka**. Na kartici **Procesi** u odjeljku **Naziv** desnom tipkom miša kliknite **Explorer**, a zatim **Ponovno pokreni**.
