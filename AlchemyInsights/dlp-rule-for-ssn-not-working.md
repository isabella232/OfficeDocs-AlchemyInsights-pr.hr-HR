---
title: DLP pravilo za SSN ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507362"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="521b6-102">DLP problemi s brojevima socijalnog osiguranja</span><span class="sxs-lookup"><span data-stu-id="521b6-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="521b6-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="521b6-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="521b6-104">**DLP problemi sa SSNs**</span><span class="sxs-lookup"><span data-stu-id="521b6-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="521b6-105">Imate li problema s **sprječavanjem gubitka podataka (DLP)** koji ne radi za sadržaj koji sadrži **broj socijalnog osiguranja (SSN)** kada koristite osjetljivu vrstu informacija u sustavu Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="521b6-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="521b6-106">Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije o tome što koristi pravilo DLP-a.</span><span class="sxs-lookup"><span data-stu-id="521b6-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="521b6-107">Na primjer, za pravilo SSN-a konfigurirano s razinom pouzdanosti od 85%, ocjenjuju se sljedeće i moraju se otkriti da bi se pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="521b6-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="521b6-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 znamenki, koje mogu biti u oblikovanom ili neoblikovanom uzorku</span><span class="sxs-lookup"><span data-stu-id="521b6-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="521b6-109">**[Uzorak:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije traže SSN-ove u četiri različita uzorka:</span><span class="sxs-lookup"><span data-stu-id="521b6-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="521b6-110">Func_ssn pronalazi SSN-ove s jakim oblikovanjem prije 2011.</span><span class="sxs-lookup"><span data-stu-id="521b6-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="521b6-111">Func_unformatted_ssn pronalazi SSN-ove s jakim oblikovanjem prije 2011.</span><span class="sxs-lookup"><span data-stu-id="521b6-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="521b6-112">Func_randomized_formatted_ssn pronalazi SSN-ove nakon 2011.</span><span class="sxs-lookup"><span data-stu-id="521b6-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="521b6-113">Func_randomized_unformatted_ssn pronalazi SSN-ove nakon 2011.</span><span class="sxs-lookup"><span data-stu-id="521b6-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="521b6-114">**[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, nema Kontrolnog zbroja.</span><span class="sxs-lookup"><span data-stu-id="521b6-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="521b6-115">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP politika je 85% sigurni da je otkrivena ova vrsta osjetljivih informacija ako, u blizini od 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="521b6-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="521b6-116">[Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) pronalazi sadržaj koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="521b6-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="521b6-117">Ključna riječ iz [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="521b6-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="521b6-118">Primjeri ključnih riječi uključuju: *socijalno osiguranje, socijalno osiguranje#, Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="521b6-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="521b6-119">Na primjer, sljedeći uzorak pokrenuo bi se za pravilo DLP SSN-a: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="521b6-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="521b6-120">Dodatne informacije o tome što je potrebno za otkrivene SSN-ove za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže SSN-ove](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="521b6-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="521b6-121">Pomoću druge ugrađene vrste osjetljivih informacija pogledajte sljedeći članak za informacije o tome što je potrebno za druge vrste: [Što traže vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="521b6-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  