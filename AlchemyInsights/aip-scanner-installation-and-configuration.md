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
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="0bc47-102">AIP Scanner: Instalacija i konfiguracija</span><span class="sxs-lookup"><span data-stu-id="0bc47-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="0bc47-103">**Da biste instalirali AIP Scanner, slijedite preporučene smjernice**:</span><span class="sxs-lookup"><span data-stu-id="0bc47-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="0bc47-104">Ako nadograđujete, a ne izvodite čistu instalaciju, provjerite jeste li slijedili smjernice za [nadogradnju skenera zaštite za Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) i za jedinstveni klijent za označavanje, pročitajte članak [Nadogradnja skenera zaštite servisa Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="0bc47-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="0bc47-105">Provjerite jeste li u skladu s [sigurnosnim vatrozidima i postavkama mrežne infrastrukture](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="0bc47-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="0bc47-106">Provjerite jesu li [pravila postavljena](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatsko označavanje ili u pravilu imaju zadanu oznaku.</span><span class="sxs-lookup"><span data-stu-id="0bc47-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="0bc47-107">Provjerite je li relevantna vrsta datoteke konfigurirana za oznaku/zaštitu kao što je opisano u [vrstama datoteka koje podržava klijent za zaštitu informacija za Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="0bc47-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="0bc47-108">Osim toga, ako želite promijeniti zadano ponašanje, slijedite ove smjernice: [Promjena zadane razine zaštite datoteka](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="0bc47-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="0bc47-109">Provjerite ima li korisnički račun konfiguriran za pokretanje servisa Scanner dozvolu za pristup svim konfiguriranim spremištima.</span><span class="sxs-lookup"><span data-stu-id="0bc47-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="0bc47-110">Ako i dalje imate problema, izvezite zapisnike skenera i dodajte ih u kartu za podršku.</span><span class="sxs-lookup"><span data-stu-id="0bc47-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="0bc47-111">**Zapisi o zaštiti podataka za izvoz servisa Azure**</span><span class="sxs-lookup"><span data-stu-id="0bc47-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="0bc47-112">Idite na%localappdata%\Microsoft\MSIP u kontekstu korisničkog konteksta koji pokreće servis skenera.</span><span class="sxs-lookup"><span data-stu-id="0bc47-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="0bc47-113">Zip svi sadržaj u mapi MSIP.</span><span class="sxs-lookup"><span data-stu-id="0bc47-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="0bc47-114">Spremite zapisnike na odabir mjesta i priložite ih na zahtjev za uslugu.</span><span class="sxs-lookup"><span data-stu-id="0bc47-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="0bc47-115">Možete koristiti i [Export-AIPLogs-Akbehalfof](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="0bc47-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="0bc47-116">**Dodatne informacije**potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="0bc47-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="0bc47-117">Implementacija skenera zaštite servisa Azure radi automatskog klasificiranje i zaštita datoteka</span><span class="sxs-lookup"><span data-stu-id="0bc47-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="0bc47-118">Određivanje i korištenje parametra tokena za set-Aipautentifikaciju</span><span class="sxs-lookup"><span data-stu-id="0bc47-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="0bc47-119">Pokretanje ciklusa otkrivanja i prikaza izvješća za skener</span><span class="sxs-lookup"><span data-stu-id="0bc47-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="0bc47-120">Pregledajte dokumentaciju o zaštiti informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="0bc47-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="0bc47-121">Preduvjeti za zaštitu informacija o Azure</span><span class="sxs-lookup"><span data-stu-id="0bc47-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="0bc47-122">Preuzimanje klijenta za zaštitu informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="0bc47-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
