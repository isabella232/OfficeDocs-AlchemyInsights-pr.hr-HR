---
title: DLP ne radi prema očekivanom
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
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977430"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="c2fee-102">DLP ne radi prema očekivanom</span><span class="sxs-lookup"><span data-stu-id="c2fee-102">DLP not working as expected</span></span>

<span data-ttu-id="c2fee-103">**Važno**: Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i onedrive ostanu vrlo dostupne – dodatne informacije [potražite u članku Prilagodbe privremenih značajki sustava SharePoint Online.](https://aka.ms/ODSPAdjustments)</span><span class="sxs-lookup"><span data-stu-id="c2fee-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="c2fee-104">**Postavljanje DLP-a**</span><span class="sxs-lookup"><span data-stu-id="c2fee-104">**Setting up DLP**</span></span>

<span data-ttu-id="c2fee-105">Imate li problema s **asprječavanjegubitka podataka (DLP)** u sustavu Office 365 koji ne funkcionira prema i očekivanom?</span><span class="sxs-lookup"><span data-stu-id="c2fee-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="c2fee-106">Ako je tako, provjerite je li **pravilo dlp-a** ispravno postavljeno i sadrže li vaši podaci ono što **pravila DLP-a** traže prilikom procjene.</span><span class="sxs-lookup"><span data-stu-id="c2fee-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="c2fee-107">DLP pravila omogućuju prepoznavanje i zaštitu osjetljivih informacija u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="c2fee-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="c2fee-108">Da biste postavili DLP pravila, koristite informacije [ovdje](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="c2fee-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="c2fee-109">**Što traže politike DLP-a**</span><span class="sxs-lookup"><span data-stu-id="c2fee-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="c2fee-110">Kada koristite **ugrađene osjetljive vrste informacija** u centru za sigurnost i usklađenost sustava Office 365, DLP pravila traže određene uzorke i elemente prilikom otkrivanja tih osjetljivih vrsta.</span><span class="sxs-lookup"><span data-stu-id="c2fee-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="c2fee-111">**Ugrađene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="c2fee-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="c2fee-112">Informacije o ugrađenim osjetljivim vrstama i što traži DLP pravilo prilikom otkrivanja osjetljive vrste [potražite u odjeljku Sljedeće koje osjetljive vrste informacija traži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="c2fee-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="c2fee-113">**Prilagođene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="c2fee-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="c2fee-114">Ako pokušavate stvoriti prilagođene vrste osjetljivih informacija, koristite sljedeći članak za informacije o stvaranju prilagođene osjetljive vrste: [Stvaranje prilagođene osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="c2fee-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="c2fee-115">**Testiranje pravila o DLP-u**</span><span class="sxs-lookup"><span data-stu-id="c2fee-115">**Test a DLP policy**</span></span>

<span data-ttu-id="c2fee-116">Da biste testirali podatke pomoću ugrađene ili prilagođene osjetljive vrste informacija, upotrijebite opciju **Vrsta testiranja** u odjeljku **Klasifikacije Osjetljive** > **vrste podataka**.</span><span class="sxs-lookup"><span data-stu-id="c2fee-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="c2fee-117">Dodatne informacije potražite [u odjeljku Testiranje prilagođenih osjetljivih vrsta informacija](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="c2fee-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="c2fee-118">**Izvješća**</span><span class="sxs-lookup"><span data-stu-id="c2fee-118">**Reports**</span></span>
  
- <span data-ttu-id="c2fee-119">Dobijte uvid u osjetljive podatke pomoću [DLP izvješća.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="c2fee-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="c2fee-120">Pogledajte specifične pojedinosti događaja s [izvješćem o incidentu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="c2fee-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
