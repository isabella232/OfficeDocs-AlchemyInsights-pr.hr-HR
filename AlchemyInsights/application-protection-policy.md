---
title: Politika zaštite aplikacija
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423333"
---
# <a name="application-protection-policy"></a>Politika zaštite aplikacija

Ako ste novi u pravilima o zaštiti aplikacija (APP), pogledajte [pregled pravila zaštite aplikacija](https://docs.microsoft.com/intune/apps/app-protection-policy).

Da biste počeli koristiti APP, [pročitajte članak Kako izraditi i dodijeliti pravila zaštite aplikacija](https://docs.microsoft.com/intune/app-protection-policies).

Zahtjevi politike zaštite aplikacija:

- Korisnik ima Intune ili EMS licencu.
- Korisnik pripada grupi koju ciljaju pravila zaštite aplikacija.
- Samo je jedan korporativni korisnik prijavljen u zaštićene aplikacije na uređaju.
- Aplikacija je implementirala [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started). Popis aplikacija koje podržavaju SDK potražite u odjeljku [Aplikacije zaštićene Microsoft Intune .](https://docs.microsoft.com/intune/apps-supported-intune-apps)

Pravila se primjenjuju nakon što korisnik koji ispunjava gore navedene zahtjeve potpiše aplikaciju s omogućenom Intune SDK-om. Najjednostavniji način za utvrđivanje primjenjuje li se pravilo tako da korisnik postavi pin u pravilima. 

Dodatne informacije potražite u članku:

[Najčešća pitanja o otklanjanju poteškoća s APP/MAM-om](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Kako provjeriti postavljanje pravila zaštite aplikacija](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Objašnjenje vremena isporuke pravila zaštite aplikacija](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Kako pratiti pravila zaštite aplikacija](https://docs.microsoft.com/intune/app-protection-policies-monitor)