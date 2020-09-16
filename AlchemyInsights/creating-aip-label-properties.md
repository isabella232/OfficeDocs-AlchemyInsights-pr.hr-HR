---
title: Stvaranje politika naljepnica u AIP-u
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732167"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="ae397-102">Stvaranje politika naljepnica u AIP-u</span><span class="sxs-lookup"><span data-stu-id="ae397-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="ae397-103">Oznake zaštite podataka Azure (AIP) mogu se koristiti s punim rasponom podataka koje tvrtka ili ustanova obično stvara i pohranjuje, od najniže klasifikacije osobnih podataka, do najviše klasifikacije vrlo povjerljivih podataka.</span><span class="sxs-lookup"><span data-stu-id="ae397-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="ae397-104">Pravilnika o zaštiti informacija za Azure primjenjuju se na klijentski alat za zaštitu od Azure (AIP), a ne za  [Ujedinjeni klijent za označavanje AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)-a.</span><span class="sxs-lookup"><span data-stu-id="ae397-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="ae397-105">U politici programa AIP možete konfigurirati više elemenata, uključujući mogućnosti kao što su:</span><span class="sxs-lookup"><span data-stu-id="ae397-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="ae397-106">Mogućnost za koju će naljepnica omogućiti administratorima ili korisniku klasificiranje i zaštitu (neobavezno) dokumente i poruke e-pošte</span><span class="sxs-lookup"><span data-stu-id="ae397-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="ae397-107">Mogućnost nametanja klasifikacije kada korisnici spremaju dokumente i šalju e-poštu</span><span class="sxs-lookup"><span data-stu-id="ae397-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="ae397-108">Mogućnost automatskog označavanja poruke e-pošte na temelju privitaka.</span><span class="sxs-lookup"><span data-stu-id="ae397-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="ae397-109">Mogućnost kontrole trake za zaštitu informacija prikazuje se u aplikacijama sustava Office</span><span class="sxs-lookup"><span data-stu-id="ae397-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="ae397-110">Dodatne mogućnosti i informacije o pravilnicima o zaštiti informacija o Azure potražite u članku: [Pregled pravilnika o zaštiti informacija za Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="ae397-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="ae397-111">Dodatne korisne resurse u vezi s politikama za AIP potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="ae397-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="ae397-112">Udžbenik: Konfiguriranje postavki pravilnika o zaštiti informacija za Azure i stvaranje nove naljepnice</span><span class="sxs-lookup"><span data-stu-id="ae397-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="ae397-113">Konfiguriranje pravilnika o zaštiti informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="ae397-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="ae397-114">Stvaranje i konfiguriranje naljepnica s osjetljivosti i njihovih pravilnika</span><span class="sxs-lookup"><span data-stu-id="ae397-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="ae397-115">Vodiči za zajednički scenariji koji koriste zaštitu informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="ae397-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="ae397-116">Pregledajte dokumentaciju o zaštiti informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="ae397-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="ae397-117">Preduvjeti za zaštitu informacija o Azure</span><span class="sxs-lookup"><span data-stu-id="ae397-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="ae397-118">Vodič za brzi početak za zaštitu informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="ae397-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="ae397-119">Preuzimanje klijenta za zaštitu informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="ae397-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)