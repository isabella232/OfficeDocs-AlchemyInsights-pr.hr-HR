---
title: DLP pravilo za SSN ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932513"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="f7fd7-102">DLP pitanja s brojevima socijalnog osiguranja</span><span class="sxs-lookup"><span data-stu-id="f7fd7-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="f7fd7-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f7fd7-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f7fd7-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f7fd7-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f7fd7-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f7fd7-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f7fd7-109">**DLP problemi sa SSN-ovima**</span><span class="sxs-lookup"><span data-stu-id="f7fd7-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="f7fd7-110">Imate li problema s **sprječavanjem gubitka podataka (DLP)** koji ne funkcionira za sadržaj koji sadrži **broj socijalnog osiguranja (SSN)** prilikom korištenja osjetljive vrste podataka u sustavu Office 365?</span><span class="sxs-lookup"><span data-stu-id="f7fd7-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="f7fd7-111">Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije za ono što traži DLP pravila.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="f7fd7-112">Na primjer, za ssn pravilo konfigurirano s razinom pouzdanosti od 85%, vrednuju se sljedeće i mora se otkriti da bi se pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="f7fd7-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="f7fd7-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 znamenki, koje mogu biti u oblikovanom ili neformatiranom uzorku</span><span class="sxs-lookup"><span data-stu-id="f7fd7-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="f7fd7-114">**[Uzorak:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije traže SSN-ove u četiri različita uzorka:</span><span class="sxs-lookup"><span data-stu-id="f7fd7-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="f7fd7-115">Func_ssn pronalazi SSN-ove s jakim oblikovanjem prije 2011.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f7fd7-116">Func_unformatted_ssn pronalazi SSN-ove s jakim oblikovanjem prije 2011.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="f7fd7-117">Func_randomized_formatted_ssn pronalazi SSN-ove za razdoblje nakon 2011.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f7fd7-118">Func_randomized_unformatted_ssn pronalazi SSN-ove nakon 2011.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="f7fd7-119">**[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, nema šah-suma.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="f7fd7-120">**[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politika je 85% uvjeren da je otkrio ovu vrstu osjetljivih informacija ako, u blizini 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="f7fd7-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f7fd7-121">[Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) pronalazi sadržaj koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="f7fd7-122">Ključna riječ iz [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) je pronađena.</span><span class="sxs-lookup"><span data-stu-id="f7fd7-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="f7fd7-123">Primjeri ključnih riječi uključuju: *socijalno osiguranje, socijalno osiguranje#, Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="f7fd7-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="f7fd7-124">Na primjer, sljedeći uzorak aktivirao bi se za politiku DLP SSN-a: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="f7fd7-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="f7fd7-125">Dodatne informacije o tome što je potrebno za otkrivenje SSN-ova za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Koje vrste osjetljivih informacija traže SSN-ove](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="f7fd7-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="f7fd7-126">Pomoću druge ugrađene osjetljive vrste informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [Što zahtijevaju osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f7fd7-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  