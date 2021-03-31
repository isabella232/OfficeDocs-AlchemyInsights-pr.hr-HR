---
title: Konfiguriranje DLP-a u krajnjim točkama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402407"
---
# <a name="configure-endpoint-dlp"></a>Konfiguriranje DLP-a u krajnjim točkama

Microsoftov DLP u krajnjim točkama omogućuje proširenje mogućnosti zaštite DLP-a i sposobnosti nadzora osjetljivih podataka na uređajima sa sustavom Windows 10. Kada se uređaji umetnu u upravljanje uređajima, možete stvoriti pravilnike o DLP-u da biste primijenili zaštitni radnje za stavke. Eksplorer za aktivnosti može se upotrebljavati za praćenje aktivnosti povjerljivih stavki. Dodatne informacije potražite u odjeljku [Uvođenje uređaja u upravljanje uređajima](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Početak rada s DLP-om u krajnjim točkama:

- Provjerite imate li odgovarajuću licencu za SKU/pretplate. Dodatne informacije potražite u članku [Licenciranje za SKU/pretplate](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Provjerite dozvole potrebne za omogućivanje upravljanja uređajima, pristup stranici za uvođenje ili uključivanje/isključivanje nadzora uređaja. Dodatne informacije potražite u članku [Dozvole](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Uvedite uređaje u upravljanje uređajima s pomoću postupka za uvođenje uređaja. Ako ne možete odabrati mogućnost uvođenja uređaja (pretpregled) u odjeljku **Postavke** usklađenosti za M365, provjerite imate li gore navedene odgovarajuće licence i dozvole. Dodatne informacije potražite u članku [Uvođenje uređaja](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Stvorite pravilnike o DLP-u radi zaštite osjetljivih stavki. Dodatne informacije potražite u [scenarijima pravilnika DLP-a za krajnje točke](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Dodatne informacije o Microsoftovom DLP-u za krajnje točke potražite u članku [Dodatne informacije o sprječavanju gubitka podataka krajnjih točaka u sustavu Microsoft 365 (pretpregled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Važni koraci za prikupljanje podataka, ako je potrebna podrška:**

1. Preuzimanje pretpregleda MDATP alata za analizu klijenta iz sustava [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Pokrenite alat kao administrator iz prozora cmd:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Kada se pojavi upit „Unesite broj minuta za prikupljanje praćenja: ”, unesite broj minuta potrebnih za pokretanje scenarija
5. Pokretanje scenarija

Prikupite izlaznu zip datoteku koja će se dati agentu za podršku.
