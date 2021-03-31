---
title: EndPoint Manager – polazišta za sigurnost
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440870"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – polazišta za sigurnost

Polazišta za sigurnost unaprijed su konfigurirane grupe postavki sustava Windows koje vam pomažu primijeniti sigurnosne postavke koje preporučuju nadležni timovi zaduženi za sigurnost. Ta se polazišta mogu prilagoditi kako bi se provele samo željene postavke i vrijednosti. Da biste saznali više informacija o polazištima za sigurnost, pročitajte članak [Upotreba polazišta za sigurnost za konfiguriranje uređaja sa sustavom Windows 10 u sustavu Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Trenutačno postoje polazišta za ove proizvode:

- Sigurnosne postavke za Windows MDM
- Sigurnost za Microsoft Defender za krajnju točku
- Microsoft Edge

Svako od polazišta redovito se ažurira i izdaje u postupnim verzijama. Svaka verzija dodaje i/ili uklanja postavke iz prethodnih verzija kako bi se osiguralo da to polazište bude u skladu s trenutačnim smjernicama. Konzola Polazišta za sigurnost u Sigurnosti krajnje točke omogućuje usporedbu različitih verzija tako što se promjene iz jedne verzije u drugu čine vidljivima.

Da biste saznali smjernice o tome kako najučinkovitije promijeniti koja se verzija polazišta implementira, pročitajte članak [Upravljanje profilima polazišta za sigurnost u sustavu Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Nakon provedbe polazišta za sigurnost možete nadzirati stanje provedbe i pregledavati postavke za svaki uređaj zasebno.

**Napomena:** kod podataka o izvješćivanju za polazišta mogu proteći do 24 sata prije no što oni budu vidljivi nakon prve provedbe na uređaju i do 6 sati za daljnja ažuriranja. 

Najčešći uzrok za to da se određena postavka polazišta ne primjenjuje jest taj što istu postavku upotrebljava drugi profil. Ovaj se scenarij može istražiti za svaki uređaj tako što će se taj uređaj odabrati iz čvora Stanje uređaja profila Polazište za sigurnost. Da biste saznali pojedinosti, pročitajte članak [Rješavanje sukoba za polazišta za sigurnost](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).