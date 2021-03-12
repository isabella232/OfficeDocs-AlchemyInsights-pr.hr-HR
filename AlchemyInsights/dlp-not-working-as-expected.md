---
title: DLP ne funkcionira kako je očekivano
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707802"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="33890-102">DLP ne funkcionira kako je očekivano</span><span class="sxs-lookup"><span data-stu-id="33890-102">DLP not working as expected</span></span>

<span data-ttu-id="33890-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="33890-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="33890-104">**Postavljanje DLP-a**</span><span class="sxs-lookup"><span data-stu-id="33890-104">**Setting up DLP**</span></span>

<span data-ttu-id="33890-105">Imate li problema s **prevencijom gubitka podataka (DLP)** u sustavu Office 365 ne funkcionira kao što ste očekivali?</span><span class="sxs-lookup"><span data-stu-id="33890-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="33890-106">Ako je tako, provjerite je li **pravilnik za DLP** ispravno postavljen i sadrže li podaci što **pravilnik o DLP** -u traži kada se ona procjenjuje.</span><span class="sxs-lookup"><span data-stu-id="33890-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="33890-107">DLP pravila omogućuju vam identifikaciju i zaštitu osjetljivih podataka u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="33890-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="33890-108">Da biste postavljanje DLP pravilnika, upotrijebite informacije [ovdje](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span><span class="sxs-lookup"><span data-stu-id="33890-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="33890-109">**Koje su politike programa DLP potražili**</span><span class="sxs-lookup"><span data-stu-id="33890-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="33890-110">Kada koristite **ugrađene vrste osjetljivih informacija** u centrima za sigurnost i usklađenost, DLP politike potražite određene obrasce i elemente prilikom otkrivanja tih osjetljivih vrsta.</span><span class="sxs-lookup"><span data-stu-id="33890-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="33890-111">**Ugrađene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="33890-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="33890-112">Informacije o ugrađenim osjetljivim vrstama i onome što funkcija DLP traži prilikom otkrivanja osjetljive vrste potražite u članku: [što vrste osjetljivih informacija traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="33890-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="33890-113">**Prilagođene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="33890-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="33890-114">Ako pokušavate stvoriti prilagođene vrste osjetljivih podataka, upotrijebite sljedeći članak da biste saznali kako stvoriti prilagođenu vrstu osjetljivog oblika: [Stvaranje prilagođene vrste osjetljivih podataka](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="33890-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="33890-115">**Testiranje pravilnika o DLP-u**</span><span class="sxs-lookup"><span data-stu-id="33890-115">**Test a DLP policy**</span></span>

<span data-ttu-id="33890-116">Da biste testirali podatke pomoću ugrađene ili prilagođene vrste osjetljivih informacija, upotrijebite mogućnost **vrsta testa** u odjeljku **razvrstavanje**  >  **osjetljivih podataka**.</span><span class="sxs-lookup"><span data-stu-id="33890-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="33890-117">Dodatne informacije potražite u članku [testiranje prilagođenih vrsta podataka koje se razlikuju](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="33890-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="33890-118">**Izvješća**</span><span class="sxs-lookup"><span data-stu-id="33890-118">**Reports**</span></span>
  
- <span data-ttu-id="33890-119">Dohvaćanje osjetljivih podataka iz uvida u [izvještaje programa DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="33890-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="33890-120">Pogledajte detaljne pojedinosti o događaju uz izvješće o [incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="33890-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
