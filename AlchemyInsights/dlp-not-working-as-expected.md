---
title: DLP ne radi prema očekivanjima
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507470"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="189ba-102">DLP ne radi prema očekivanjima</span><span class="sxs-lookup"><span data-stu-id="189ba-102">DLP not working as expected</span></span>

<span data-ttu-id="189ba-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="189ba-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="189ba-104">**Postavljanje DLP-a**</span><span class="sxs-lookup"><span data-stu-id="189ba-104">**Setting up DLP**</span></span>

<span data-ttu-id="189ba-105">Imate li problema sa **sprječavanjem gubitka podataka (DLP)** u sustavu Office 365 koji ne funkcioniraju prema očekivanjima?</span><span class="sxs-lookup"><span data-stu-id="189ba-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="189ba-106">Ako je tako, provjerite je li **pravilo DLP** ispravno postavljeno i sadrži li vaši podaci ono što **pravilo DLP-a** traži prilikom procjene.</span><span class="sxs-lookup"><span data-stu-id="189ba-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="189ba-107">DLP pravila omogućuju vam prepoznavanje i zaštitu osjetljivih podataka u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="189ba-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="189ba-108">Da biste postavili DLP pravila, ovdje koristite [informacije](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="189ba-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="189ba-109">**Što DLP politike traže**</span><span class="sxs-lookup"><span data-stu-id="189ba-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="189ba-110">Kada koristite **ugrađene vrste osjetljivih informacija** u centrima za sigurnost i usklađenost, DLP pravila traže određene uzorke i elemente prilikom otkrivanja tih osjetljivih vrsta.</span><span class="sxs-lookup"><span data-stu-id="189ba-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="189ba-111">**Ugrađene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="189ba-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="189ba-112">Informacije o ugrađenim osjetljivim vrstama i što DLP pravilo traži prilikom otkrivanja vrste Osjetljivo [potražite u odjeljku Što traže vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="189ba-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="189ba-113">**Prilagođene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="189ba-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="189ba-114">Ako pokušavate stvoriti prilagođene vrste osjetljivih informacija, koristite sljedeći članak za informacije o stvaranju prilagođene osjetljive vrste: [Stvaranje prilagođene vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="189ba-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="189ba-115">**Testiranje pravila O DLP-u**</span><span class="sxs-lookup"><span data-stu-id="189ba-115">**Test a DLP policy**</span></span>

<span data-ttu-id="189ba-116">Da biste testirali podatke s ugrađenom ili prilagođenom osjetljivom vrstom informacija, upotrijebite mogućnost **Vrsta testiranja** u odjeljku **Vrste osjetljivih podataka Klasifikacije**  >  **Sensitive info types**.</span><span class="sxs-lookup"><span data-stu-id="189ba-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="189ba-117">Dodatne informacije potražite u [odjeljku Testiranje prilagođenih vrsta osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="189ba-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="189ba-118">**Izvješća**</span><span class="sxs-lookup"><span data-stu-id="189ba-118">**Reports**</span></span>
  
- <span data-ttu-id="189ba-119">Dobijte osjetljive uvide u podatke pomoću [DLP izvješća.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="189ba-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="189ba-120">Pogledajte određene pojedinosti događaja pomoću [izvješća o incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="189ba-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
