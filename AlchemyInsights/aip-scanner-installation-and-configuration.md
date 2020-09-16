---
title: 'AIP Scanner: Instalacija i konfiguracija'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686634"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP Scanner: Instalacija i konfiguracija

**Da biste instalirali AIP Scanner, slijedite preporučene smjernice**:

1. Ako nadograđujete, a ne izvodite čistu instalaciju, provjerite jeste li slijedili smjernice za [nadogradnju skenera zaštite za Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) i za jedinstveni klijent za označavanje, pročitajte članak [Nadogradnja skenera zaštite servisa Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Provjerite jeste li u skladu s [sigurnosnim vatrozidima i postavkama mrežne infrastrukture](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Provjerite jesu li [pravila postavljena](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatsko označavanje ili u pravilu imaju zadanu oznaku.
4. Provjerite je li relevantna vrsta datoteke konfigurirana za oznaku/zaštitu kao što je opisano u [vrstama datoteka koje podržava klijent za zaštitu informacija za Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Osim toga, ako želite promijeniti zadano ponašanje, slijedite ove smjernice: [Promjena zadane razine zaštite datoteka](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Provjerite ima li korisnički račun konfiguriran za pokretanje servisa Scanner dozvolu za pristup svim konfiguriranim spremištima.
6. Ako i dalje imate problema, izvezite zapisnike skenera i dodajte ih u kartu za podršku.

**Zapisi o zaštiti podataka za izvoz servisa Azure**

1. Idite na%localappdata%\Microsoft\MSIP u kontekstu korisničkog konteksta koji pokreće servis skenera.
2. Zip svi sadržaj u mapi MSIP.
3. Spremite zapisnike na odabir mjesta i priložite ih na zahtjev za uslugu.
4. Možete koristiti i [Export-AIPLogs-Akbehalfof](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Dodatne informacije**potražite u članku:
- [Implementacija skenera zaštite servisa Azure radi automatskog klasificiranje i zaštita datoteka](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Određivanje i korištenje parametra tokena za set-Aipautentifikaciju](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Pokretanje ciklusa otkrivanja i prikaza izvješća za skener](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Pregledajte dokumentaciju o zaštiti informacija za Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Preduvjeti za zaštitu informacija o Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Preuzimanje klijenta za zaštitu informacija za Azure](https://www.microsoft.com/download/details.aspx?id=53018)
