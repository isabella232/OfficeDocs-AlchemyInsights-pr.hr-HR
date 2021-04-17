---
title: 'AIP skener: instalacija i konfiguracija'
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821655"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP skener: instalacija i konfiguracija

**Da biste instalirali AIP skener, slijedite preporučene smjernice:**

1. Ako nadograđujete i ne izvodite čistu instalaciju, provjerite jeste li pratili smjernice za nadogradnju skenera [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) i klijenta za sjedinjeno označavanje, pročitajte nadogradnju skenera Azure Information [Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Provjerite jeste li usklađeni sa svim [preduvjetima za postavke vatrozida i mrežne infrastrukture](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Provjerite jesu li [vaši pravilniki postavljeni](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatsko označavanje ili imaju zadanu oznaku u pravilniku.
4. Provjerite je li odgovarajuća vrsta datoteke konfigurirana za oznaku/zaštitu na način opisan u [odjeljku](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)Vrste datoteka koje podržava klijent azure Information Protection . Osim toga, ako želite promijeniti zadano ponašanje, slijedite ove smjernice: [Promjena zadane razine zaštite datoteka](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Provjerite ima li korisnički račun konfiguriran za pokretanje servisa skenera dozvole za pristup svim konfiguriranim spremištima.
6. Ako i dalje imate problema, izvezite zapisnike skenera i dodajte ih na kartu za podršku.

**Izvoz zapisnika skenera za zaštitu podataka na servisu Azure**

1. Idite na %localappdata%\Microsoft\MSIP u kontekstu korisnika koji izvodi servis skenera.
2. Zip all the contents under the MSIP folder.
3. Spremite zapisnike na odabir lokacije i priložite ih zahtjevu za uslugu.
4. Možete koristiti i [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Dodatne informacije potražite u članku**:
- [Implementacija skenera Azure Information Protection radi automatskog klasificiranja i zaštite datoteka](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Određivanje i korištenje parametra Token za Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Pokretanje ciklusa otkrivanja i prikaz izvješća za skener](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Pregled dokumentacije za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Preduvjeti za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Preuzimanje klijenta za Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
