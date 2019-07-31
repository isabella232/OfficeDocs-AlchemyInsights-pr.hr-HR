---
title: DLP ne funkcioniraju prema očekivanjima
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941060"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="aac14-102">DLP ne funkcioniraju prema očekivanjima</span><span class="sxs-lookup"><span data-stu-id="aac14-102">DLP not working as expected</span></span>

<span data-ttu-id="aac14-103">Imate problema s **Podataka gubitak Data Execution Prevention (DLP)** u sustavu Office 365 ne funkcioniraju prema očekivanjima?</span><span class="sxs-lookup"><span data-stu-id="aac14-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="aac14-104">Ako je tako, provjerite **pravila DLP** ispravno postavili, a podaci sadrže **pravila DLP** je tražite kada je procjene.</span><span class="sxs-lookup"><span data-stu-id="aac14-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="aac14-105">**Postavljanje DLP**</span><span class="sxs-lookup"><span data-stu-id="aac14-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="aac14-106">DLP pravila omogućuje prepoznavanje i zaštitite osjetljive informacije u organizaciji.</span><span class="sxs-lookup"><span data-stu-id="aac14-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="aac14-107">Za postavljanje DLP pravilima, koristite informacije [ovdje](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="aac14-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="aac14-108">**Što DLP pravila izgleda**</span><span class="sxs-lookup"><span data-stu-id="aac14-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="aac14-109">Kada koristite **vrste ugrađene osjetljive informacije** u centru sigurnosti Office 365 i usklađenosti DLP pravila izgledati za određene Uzorci i elemente otkrivanje te osjetljive vrste.</span><span class="sxs-lookup"><span data-stu-id="aac14-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="aac14-110">**Vrste ugrađene osjetljive informacije**</span><span class="sxs-lookup"><span data-stu-id="aac14-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="aac14-111">Informacije o ugrađene osjetljive vrste i što DLP pravila traži kada otkrivanje osjetljivih vrsta potražite: [potražite kakve osjetljive informacije](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="aac14-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="aac14-112">**Vrste prilagođenih osjetljive informacije**</span><span class="sxs-lookup"><span data-stu-id="aac14-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="aac14-113">Ako pokušavate stvoriti vrste prilagođenih osjetljive informacije, koristite sljedeći članak za informacije o tome kako stvoriti prilagođenu vrstu osjetljive: [Stvaranje prilagođenih osjetljive informacije vrsta](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="aac14-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="aac14-114">**Testiranje pravila DLP**</span><span class="sxs-lookup"><span data-stu-id="aac14-114">**Test a DLP policy**</span></span>

<span data-ttu-id="aac14-115">Za testiranje podataka s vrstom ugrađene ili prilagođene osjetljive informacije, koristite mogućnost **testiranje vrsta** pod **klasifikacije** > **vrste osjetljivih informacija**.</span><span class="sxs-lookup"><span data-stu-id="aac14-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="aac14-116">Za dodatne informacije pogledajte [Test vrste prilagođenih osjetljive informacije](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="aac14-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="aac14-117">**Izvješća**</span><span class="sxs-lookup"><span data-stu-id="aac14-117">**Reports**</span></span>
  
- <span data-ttu-id="aac14-118">Dohvati osjetljive podatke uvida s [izvješća o DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="aac14-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="aac14-119">Vidjeti određene detalje događaja s [Izvješće Incident](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="aac14-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
