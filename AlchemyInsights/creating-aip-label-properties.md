---
title: Stvaranje pravila AIP oznake
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44568958"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="110f5-102">Stvaranje pravila AIP oznake</span><span class="sxs-lookup"><span data-stu-id="110f5-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="110f5-103">Oznake Azure Information Protection(AIP) mogu se koristiti s cijelim rasponom podataka koje organizacija obično stvara i pohranjuje, od najniže klasifikacije osobnih podataka, do najviše klasifikacije vrlo povjerljivih podataka.</span><span class="sxs-lookup"><span data-stu-id="110f5-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="110f5-104">Pravila zaštite podataka azure primjenjuju se na klasični klijent Azure Information Protection(AIP), a ne na [klijent za objedinjavanje AIP-a](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="110f5-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="110f5-105">Možete konfigurirati više elemenata u AIP pravilima, uključujući opcije kao što su:</span><span class="sxs-lookup"><span data-stu-id="110f5-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="110f5-106">Opcija za koju će oznaka administratorima ili korisniku dopustiti klasifikaciju i zaštitu (neobavezne) dokumente i e-poštu</span><span class="sxs-lookup"><span data-stu-id="110f5-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="110f5-107">Mogućnost provođenja klasifikacije prilikom spremanja dokumenata i slanja e-pošte</span><span class="sxs-lookup"><span data-stu-id="110f5-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="110f5-108">Mogućnost automatskog označavanja poruke e-pošte na temelju njezinih privitaka.</span><span class="sxs-lookup"><span data-stu-id="110f5-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="110f5-109">Mogućnost kontrole prikazuje li se traka Zaštita informacija u aplikacijama sustava Office</span><span class="sxs-lookup"><span data-stu-id="110f5-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="110f5-110">Dodatne mogućnosti i informacije o pravilima zaštite podataka azure potražite u članku [Pregled pravila zaštite podataka azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="110f5-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="110f5-111">Za druge korisne resurse u vezi s AIP pravilima pogledajte:</span><span class="sxs-lookup"><span data-stu-id="110f5-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="110f5-112">Vodič: Konfiguriranje postavki pravila zaštite podataka za Azure i stvaranje nove oznake</span><span class="sxs-lookup"><span data-stu-id="110f5-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="110f5-113">Konfiguriranje pravila zaštite podataka za Azure</span><span class="sxs-lookup"><span data-stu-id="110f5-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="110f5-114">Stvaranje i konfiguriranje oznaka osjetljivosti i njihovih pravila</span><span class="sxs-lookup"><span data-stu-id="110f5-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="110f5-115">Upute za uobičajene scenarije koji koriste Azure information protection</span><span class="sxs-lookup"><span data-stu-id="110f5-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="110f5-116">Pregled dokumentacije o zaštiti podataka za Azure</span><span class="sxs-lookup"><span data-stu-id="110f5-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="110f5-117">Zahtjevi za zaštitu informacija azure</span><span class="sxs-lookup"><span data-stu-id="110f5-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="110f5-118">Vodič za brzi početak zaštite informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="110f5-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="110f5-119">Preuzimanje klijenta za zaštitu podataka za Azure</span><span class="sxs-lookup"><span data-stu-id="110f5-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)