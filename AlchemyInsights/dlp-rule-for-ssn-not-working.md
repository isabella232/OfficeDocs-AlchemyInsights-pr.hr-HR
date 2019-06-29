---
title: DLP pravilo za MBG ne radi
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
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389425"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="d2af4-102">DLP problemi s brojeva socijalnog osiguranja</span><span class="sxs-lookup"><span data-stu-id="d2af4-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="d2af4-103">Imate li problema s **Podataka gubitak Data Execution Prevention (DLP)** za sadržaj koji sadrži **Broj socijalnog osiguranja (MBG)** kada koristite vrstu osjetljive informacije u Office 365 ne radi?</span><span class="sxs-lookup"><span data-stu-id="d2af4-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="d2af4-104">Ako je tako, provjerite je li vaš sadržaj sadrži potrebne informacije za što pravila DLP izgleda.</span><span class="sxs-lookup"><span data-stu-id="d2af4-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="d2af4-105">Ako, na primjer, za MBG pravila konfigurirana s razinu pouzdanosti 85%, sljedeće vrednuju i morate otkrio za pravilo okidač:</span><span class="sxs-lookup"><span data-stu-id="d2af4-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d2af4-106">**[Oblik:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 znamenki, što može biti oblikovani ili neoblikovani uzorak</span><span class="sxs-lookup"><span data-stu-id="d2af4-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="d2af4-107">**[Uzorak:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije Potraži SSNs četiri različite uzorci:</span><span class="sxs-lookup"><span data-stu-id="d2af4-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="d2af4-108">Func_ssn pronalazi SSNs s pre 2011 Snažno oblikovanje koje su oblikovane tim crtice ili razmaka (ddd dd dddd ili ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="d2af4-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d2af4-109">Func_unformatted_ssn pronalazi SSNs s pre 2011 Snažno oblikovanje koje su Neoblikovani kao devet uzastopne znamenke (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="d2af4-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="d2af4-110">Func_randomized_formatted_ssn pronalazi Proknjiži 2011 SSNs koji su oblikovani crtice ili razmaka (ddd dd dddd ili ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="d2af4-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d2af4-111">Func_randomized_unformatted_ssn pronalazi Proknjiži 2011 SSNs koje su Neoblikovani kao devet uzastopne znamenke (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="d2af4-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="d2af4-112">**[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne postoji nijedan kontrolni zbroj</span><span class="sxs-lookup"><span data-stu-id="d2af4-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="d2af4-113">**[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP pravila je % 85 sigurni da je otkrio ovu vrstu osjetljive informacije ako unutar blizine 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="d2af4-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d2af4-114">[Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) pronalazi sadržaja koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="d2af4-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d2af4-115">Ključne riječi iz [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) nije pronađen.</span><span class="sxs-lookup"><span data-stu-id="d2af4-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="d2af4-116">Primjeri ključne riječi uključuje: *JMBG, JMBG #, PnP sek, zdravstvene Iskaznice* .</span><span class="sxs-lookup"><span data-stu-id="d2af4-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="d2af4-117">Ako, na primjer, sljedeći uzorak 'D okidač MBG DLP pravila: **MBG: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="d2af4-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="d2af4-118">Dodatne informacije na što je potrebno za SSNs otkrio za sadržaj potražite u sljedećoj sekciji ovog članka: [Što u osjetljive informacije vrste izgledaju SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="d2af4-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="d2af4-119">Pomoću različitih osjetljivih informacija za ugrađene vrste, pogledajte sljedeći članak informacije na što je potrebno za druge vrste: [što u osjetljive informacije vrste Potraži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d2af4-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  