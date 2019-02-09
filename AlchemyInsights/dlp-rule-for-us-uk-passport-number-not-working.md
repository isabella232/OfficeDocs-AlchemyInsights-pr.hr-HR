---
title: DLP pravilo za SAD / velika Britanija Passport broj ne radi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: ec7f11676982b56a46c83bf276c2212ce765ba6f
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786690"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="2d2de-102">Problemi s DLP - sad / brojevi Passport velika Britanija</span><span class="sxs-lookup"><span data-stu-id="2d2de-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="2d2de-p101">Imate problema s **Podataka gubitak Data Execution Prevention (DLP)** ne rade za sadržaja koji sadrži na **sad / velika Britanija Passport broj** prilikom korištenja vrsta osjetljive informacije DLP u O365? Ako je tako, provjerite je li vaš sadržaj sadrži potrebne informacije za što je tražite pravila DLP prilikom procjene.</span><span class="sxs-lookup"><span data-stu-id="2d2de-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="2d2de-105">Na primjer, za na **sad / velika Britanija Passport broj** pravila konfiguriran s razinu pouzdanosti 75% sljedeće vrednuju i morate otkrio za pravilo okidač</span><span class="sxs-lookup"><span data-stu-id="2d2de-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="2d2de-106">**[Obliku:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devet znamenki</span><span class="sxs-lookup"><span data-stu-id="2d2de-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="2d2de-107">**[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devet uzastopne znamenki</span><span class="sxs-lookup"><span data-stu-id="2d2de-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="2d2de-108">**[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne postoji nijedan kontrolni zbroj</span><span class="sxs-lookup"><span data-stu-id="2d2de-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="2d2de-109">**[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Pravila DLP je 75% sigurni da je otkrio ovu vrstu osjetljive informacije ako unutar blizine 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="2d2de-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="2d2de-110">Funkcija Func_usa_uk_passport pronalazi sadržaja koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="2d2de-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="2d2de-111">Ključne riječi iz Keyword_passport nije pronađen.</span><span class="sxs-lookup"><span data-stu-id="2d2de-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="2d2de-112">Ako, na primjer, sljedeći uzorak bi okidač za u **sad / velika Britanija Passport broj** pravila: SAD Passport broj 123456789</span><span class="sxs-lookup"><span data-stu-id="2d2de-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="2d2de-113">Dodatne informacije na što je potrebno za u SAD / velika Britanija Passport broj otkrio za sadržaj, pogledajte sljedeći odjeljak u ovom članku: [što u osjetljive informacije vrste izgleda za SAD / velika Britanija Passport broj](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="2d2de-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="2d2de-114">Pomoću različitih osjetljivih informacija za ugrađene vrste, pogledajte sljedeći članak informacije na što je potrebno za druge vrste: [što u osjetljive informacije vrste Potraži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="2d2de-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

