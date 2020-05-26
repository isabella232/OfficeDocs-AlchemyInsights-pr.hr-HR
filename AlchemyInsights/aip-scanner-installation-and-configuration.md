---
title: 'AIP skener: instalacija i konfiguracija'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357463"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP skener: instalacija i konfiguracija

**Da biste instalirali AIP skener, slijedite preporučene smjernice:**

1. Ako nadograđujete i ne obavljate čistu instalaciju, provjerite jeste li slijedili smjernice za [nadogradnju skenera Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) i za objedinjeno označavanje klijenta, pogledajte nadogradnju [skenera Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Provjerite jeste li u skladu sa svim [preduvjetima za postavke vatrozida i mrežne infrastrukture](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Provjerite jesu li [pravila postavljena](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatsko označavanje ili imaju li u pravilima zadanu oznaku.
4. Provjerite je li odgovarajuća vrsta datoteke konfigurirana za označavanje/zaštitu kako je opisano u [vrstama datoteka koje podržava klijent Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Osim toga, ako želite promijeniti zadano ponašanje, slijedite ove smjernice: [Promjena zadane razine zaštite datoteka](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Provjerite ima li korisnički račun konfiguriran za pokretanje servisa skenera dozvole za pristup svim konfiguriranim spremištima.
6. Ako i dalje imate problema, izvezite zapisnike skenera i dodajte ih na svoju ulaznicu za podršku.

**Izvoz zapisnika skenera azure zaštite podataka**

1. Idite na %localappdata%\Microsoft\MSIP pod kontekstom korisnika koji pokreće servis skenera.
2. Zip sve sadržaje ispod MSIP mape.
3. Spremite zapisnike na svoju lokaciju i priložite ih zahtjevu za uslugom.
4. Možete koristiti [i Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Dodatne informacije potražite u odjeljku**:
- [Uvođenje skenera azure information protection za automatsko razvrstavanje i zaštitu datoteka](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Određivanje i korištenje parametra tokena za Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Pokretanje ciklusa otkrivanja i prikaz izvješća za skener](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Pregled dokumentacije o zaštiti informacija na servisu Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Preduvjeti za azure zaštitu informacija](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Preuzmite klijent azure zaštite informacija](https://www.microsoft.com/download/details.aspx?id=53018)
