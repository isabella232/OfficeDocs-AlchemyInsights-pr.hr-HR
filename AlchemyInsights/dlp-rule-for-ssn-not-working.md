---
title: DLP pravilo za SSN ne funkcionira
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679361"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="e1073-102">DLP problemi s brojevima socijalnog osiguranja</span><span class="sxs-lookup"><span data-stu-id="e1073-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="e1073-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="e1073-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="e1073-104">**DLP problemi s SSN-om**</span><span class="sxs-lookup"><span data-stu-id="e1073-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="e1073-105">Imate li problema s **prevencijom gubitka podataka (DLP)** ne radi za sadržaj koji sadrži **broj socijalnog osiguranja (SSN)** kada koristite vrstu osjetljive informacije u programu Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="e1073-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="e1073-106">Ako je tako, provjerite sadrži li sadržaj potrebne informacije o tome što pravilnik programa DLP traži.</span><span class="sxs-lookup"><span data-stu-id="e1073-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="e1073-107">Primjerice, ako je pravilo SSN konfigurirano uz razinu pouzdanosti od 85%, procjenjuje se sljedeće i mora se otkriti da bi se pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="e1073-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="e1073-108">**[Oblik:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 znamenaka, koje se mogu oblikovati u oblikovani ili neoblikovani uzorak</span><span class="sxs-lookup"><span data-stu-id="e1073-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="e1073-109">**[Uzorak:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije traže SSN-ove u četiri različita uzorka:</span><span class="sxs-lookup"><span data-stu-id="e1073-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="e1073-110">Func_ssn pronalazi SSN-ove s pret2011 snažnim oblikovanjem koje su oblikovane crtice ili razmaci (DDD-DD-dddd ili DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="e1073-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="e1073-111">Func_unformatted_ssn pronalazi SSN-ove s pret2011 jakim oblikovanjem koje su neoblikovane kao devet uzastopnih znamenki (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="e1073-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="e1073-112">Func_randomized_formatted_ssn pronalazi SSN-ove za post-2011 koje su oblikovane crtice ili razmaci (DDD-DD-dddd ili DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="e1073-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="e1073-113">Func_randomized_unformatted_ssn pronalazi SSN-ove post-2011 koji su neoblikovani kao devet uzastopnih znamenki (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="e1073-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="e1073-114">**[Potvrdni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, ne postoji checksum</span><span class="sxs-lookup"><span data-stu-id="e1073-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="e1073-115">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP pravilo je 85% pouzdano da je otkrivena ta vrsta osjetljivih podataka ako je u neposrednoj blizini znakova od 300:</span><span class="sxs-lookup"><span data-stu-id="e1073-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="e1073-116">[Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) pronalazi sadržaj koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="e1073-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="e1073-117">Pronađena je ključna riječ iz [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="e1073-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="e1073-118">Primjeri ključnih riječi obuhvaća:  *socijalna sigurnost, socijalna sigurnost #, soc sec, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="e1073-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="e1073-119">Na primjer, sljedeći će se uzorak pokrenuti za pravilnik o DLP SSN-u: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="e1073-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="e1073-120">Dodatne informacije o tome što je potrebno za prezentacije za SSN-ovi za sadržaj potražite u sljedećem odjeljku u ovom članku: [što vrste osjetljivih informacija traže SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) -ove</span><span class="sxs-lookup"><span data-stu-id="e1073-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="e1073-121">Korištenje različitih ugrađenih vrsta osjetljivih informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [što vrste osjetljivih podataka traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="e1073-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  