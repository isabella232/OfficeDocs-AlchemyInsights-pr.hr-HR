---
title: DLP pravilo za MBG ne radi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404409"
---
<span data-ttu-id="a6d33-102">Imate li problema s **Podataka gubitak Data Execution Prevention (DLP)** za sadržaj koji sadrži **Broj socijalnog osiguranja (MBG)** kada koristite vrstu osjetljive informacije u Office 365 ne radi?</span><span class="sxs-lookup"><span data-stu-id="a6d33-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="a6d33-103">Ako je tako, provjerite je li vaš sadržaj sadrži potrebne informacije za što pravila DLP izgleda.</span><span class="sxs-lookup"><span data-stu-id="a6d33-103">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="a6d33-104">Ako, na primjer, za MBG pravila konfigurirana s razinu pouzdanosti 85%, sljedeće vrednuju i morate otkrio za pravilo okidač:</span><span class="sxs-lookup"><span data-stu-id="a6d33-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a6d33-105">**[Oblik:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 znamenki, što može biti oblikovani ili neoblikovani uzorak</span><span class="sxs-lookup"><span data-stu-id="a6d33-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="a6d33-106">**[Uzorak:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije Potraži SSNs četiri različite uzorci:</span><span class="sxs-lookup"><span data-stu-id="a6d33-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="a6d33-107">Func_ssn pronalazi SSNs s pre 2011 Snažno oblikovanje koje su oblikovane tim crtice ili razmaka (ddd dd dddd ili ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="a6d33-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="a6d33-108">Func_unformatted_ssn pronalazi SSNs s pre 2011 Snažno oblikovanje koje su Neoblikovani kao devet uzastopne znamenke (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="a6d33-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="a6d33-109">Func_randomized_formatted_ssn pronalazi Proknjiži 2011 SSNs koji su oblikovani crtice ili razmaka (ddd dd dddd ili ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="a6d33-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="a6d33-110">Func_randomized_unformatted_ssn pronalazi Proknjiži 2011 SSNs koje su Neoblikovani kao devet uzastopne znamenke (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="a6d33-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="a6d33-111">**[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne postoji nijedan kontrolni zbroj</span><span class="sxs-lookup"><span data-stu-id="a6d33-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="a6d33-112">**[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP pravila je % 85 sigurni da je otkrio ovu vrstu osjetljive informacije ako unutar blizine 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="a6d33-112">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="a6d33-113">[Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) pronalazi sadržaja koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="a6d33-113">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="a6d33-114">Ključne riječi iz [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) nije pronađen.</span><span class="sxs-lookup"><span data-stu-id="a6d33-114">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="a6d33-115">Primjeri ključne riječi uključuje: *JMBG, JMBG #, PnP sek, zdravstvene Iskaznice* .</span><span class="sxs-lookup"><span data-stu-id="a6d33-115">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="a6d33-116">Ako, na primjer, sljedeći uzorak 'D okidač MBG DLP pravila: **MBG: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="a6d33-116">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="a6d33-117">Dodatne informacije na što je potrebno za SSNs otkrio za sadržaj potražite u sljedećoj sekciji ovog članka: [Što u osjetljive informacije vrste izgledaju SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="a6d33-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="a6d33-118">Pomoću različitih osjetljivih informacija za ugrađene vrste, pogledajte sljedeći članak informacije na što je potrebno za druge vrste: [što u osjetljive informacije vrste Potraži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a6d33-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

