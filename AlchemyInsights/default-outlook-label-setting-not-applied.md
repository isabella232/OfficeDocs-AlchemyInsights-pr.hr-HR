---
title: Zadana Outlook naljepnica nije primijenjena
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454480"
---
# <a name="default-outlook-label-setting-not-applied"></a>Zadana Outlook naljepnica nije primijenjena

Ako se zadane Outlook naljepnice ne primjenjuju pravilno i primjenjuje se druga naljepnica ili bez oznake, možda nailazite na poznati problem (MC277818) i trebali biste učiniti jednu od ove dvije mogućnosti da biste riješili problem:

**Prva mogućnost:**

1. Idite na Microsoft 365 centar za usklađenost > **rješenja za**  >  **zaštitu informacija**.
1. Odaberite **Pravila naljepnica**, a zatim odaberite pravilnik naljepnica koji morate urediti **(postavka oznake OutlookDefaultlabel** nije pravilno postavljena na odgovarajućem pravilniku za naljepnice. Pokrenite **Get-labelpolicy da** biste prikazali tu postavku), a zatim **odaberite Uređivanje pravilnika**.
1. Odaberite **Dalje** dok ne vidite postavku Primijeni tu zadanu oznaku na poruke e-pošte **,** koja je dostupna ako odaberete Zatraži od korisnika primjenu oznake na **e-poštu** i dokumente nasljednika u **dijaloškom** okviru Postavke pravilnika.
1. U **dijaloškom okviru Primjena zadane oznake na** dokumente na padajući **popis** odaberite Ništa.
1. Odaberite **Dalje** **i Pošalji da** biste spremili postavke naljepnice.

**Druga mogućnost:**

U centru za sigurnost i usklađenost [powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)koristite naredbeni Set-LabelPolicy da biste **outlookDefaultlabel** promijenili u Ništa **na** servisu {OutlookDefaultLabel="None"}.

Pokreni: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Dodatne informacije o zadanim naljepnicama za Outlook potražite u članku [Postavljanje druge zadane oznake za Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).