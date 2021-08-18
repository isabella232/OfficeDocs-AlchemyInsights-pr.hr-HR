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
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323910"
---
# <a name="configure-endpoint-dlp"></a>Konfiguriranje DLP-a u krajnjim točkama

Microsoftov DLP u krajnjim točkama omogućuje proširenje mogućnosti zaštite DLP-a i sposobnosti nadzora osjetljivih podataka na uređajima sa sustavom Windows 10. Kada se uređaji umetnu u upravljanje uređajima, možete stvoriti pravilnike o DLP-u da biste primijenili zaštitni radnje za stavke. Eksplorer za aktivnosti može se upotrebljavati za praćenje aktivnosti povjerljivih stavki. Dodatne informacije potražite u odjeljku [Uvođenje uređaja u upravljanje uređajima](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Početak rada s DLP-om u krajnjim točkama:

- Provjerite imate li odgovarajuću licencu za SKU/pretplate. Dodatne informacije potražite u članku [Licenciranje za SKU/pretplate](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Provjerite dozvole potrebne za omogućivanje upravljanja uređajima, pristup stranici za uvođenje ili uključivanje/isključivanje nadzora uređaja. Dodatne informacije potražite u članku [Dozvole](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Uvedite uređaje u upravljanje uređajima s pomoću postupka za uvođenje uređaja. Dodatne informacije potražite u članku [Uvođenje uređaja](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Stvorite pravilnike o DLP-u radi zaštite osjetljivih stavki. Dodatne informacije potražite u [scenarijima pravilnika DLP-a za krajnje točke](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Dodatne informacije o Microsoftovom DLP-u za krajnje točke potražite u članku [Dodatne informacije o sprječavanju gubitka podataka krajnjih točaka u sustavu Microsoft 365 (pretpregled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Važni koraci za prikupljanje podataka, ako je potrebna podrška:**

1. Preuzimanje [pretpregleda alata za analizu klijenta za MDATP](https://aka.ms/betamdatpanalyzer).
1. Pokrenite alat kao administrator iz prozora cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Kada se od vas zatraži **da unesete broj minuta** za prikupljanje praćenja: unesite broj minuta potrebnih za pokretanje scenarija.
1. Pokrenite scenarij.

Prikupite izlaz zip datoteke koji želite dati agentu za podršku.
