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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932614"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="06992-102">DLP ne radi prema očekivanom</span><span class="sxs-lookup"><span data-stu-id="06992-102">DLP not working as expected</span></span>

<span data-ttu-id="06992-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="06992-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="06992-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="06992-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="06992-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="06992-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="06992-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="06992-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="06992-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="06992-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="06992-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="06992-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="06992-109">**Postavljanje DLP-a**</span><span class="sxs-lookup"><span data-stu-id="06992-109">**Setting up DLP**</span></span>

<span data-ttu-id="06992-110">Imate li problema s **asprječavanjegubitka podataka (DLP)** u sustavu Office 365 koji ne funkcionira prema i očekivanom?</span><span class="sxs-lookup"><span data-stu-id="06992-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="06992-111">Ako je tako, provjerite je li **pravilo dlp-a** ispravno postavljeno i sadrže li vaši podaci ono što **pravila DLP-a** traže prilikom procjene.</span><span class="sxs-lookup"><span data-stu-id="06992-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="06992-112">DLP pravila omogućuju prepoznavanje i zaštitu osjetljivih informacija u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="06992-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="06992-113">Da biste postavili DLP pravila, koristite informacije [ovdje](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="06992-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="06992-114">**Što traže politike DLP-a**</span><span class="sxs-lookup"><span data-stu-id="06992-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="06992-115">Kada koristite **ugrađene osjetljive vrste informacija** u centru za sigurnost i usklađenost sustava Office 365, DLP pravila traže određene uzorke i elemente prilikom otkrivanja tih osjetljivih vrsta.</span><span class="sxs-lookup"><span data-stu-id="06992-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="06992-116">**Ugrađene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="06992-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="06992-117">Informacije o ugrađenim osjetljivim vrstama i što traži DLP pravilo prilikom otkrivanja osjetljive vrste [potražite u odjeljku Sljedeće koje osjetljive vrste informacija traži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="06992-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="06992-118">**Prilagođene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="06992-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="06992-119">Ako pokušavate stvoriti prilagođene vrste osjetljivih informacija, koristite sljedeći članak za informacije o stvaranju prilagođene osjetljive vrste: [Stvaranje prilagođene osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="06992-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="06992-120">**Testiranje pravila o DLP-u**</span><span class="sxs-lookup"><span data-stu-id="06992-120">**Test a DLP policy**</span></span>

<span data-ttu-id="06992-121">Da biste testirali podatke pomoću ugrađene ili prilagođene osjetljive vrste informacija, upotrijebite opciju **Vrsta testiranja** u odjeljku **Klasifikacije Osjetljive** > **vrste podataka**.</span><span class="sxs-lookup"><span data-stu-id="06992-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="06992-122">Dodatne informacije potražite [u odjeljku Testiranje prilagođenih osjetljivih vrsta informacija](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="06992-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="06992-123">**Izvješća**</span><span class="sxs-lookup"><span data-stu-id="06992-123">**Reports**</span></span>
  
- <span data-ttu-id="06992-124">Dobijte uvid u osjetljive podatke pomoću [DLP izvješća.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="06992-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="06992-125">Pogledajte specifične pojedinosti događaja s [izvješćem o incidentu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="06992-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
