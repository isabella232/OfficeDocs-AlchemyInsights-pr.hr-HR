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
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790540"
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
