---
title: DLP pravilo za broj kreditne kartice ne radi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404473"
---
<span data-ttu-id="945d4-102">Imate li problema s **Podataka gubitak Data Execution Prevention (DLP)** ne rade za sadržaj koji sadrži **Broj kreditne kartice** kada koristite vrstu osjetljive informacije DLP u O365?</span><span class="sxs-lookup"><span data-stu-id="945d4-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="945d4-103">Ako je tako, provjerite je li vaš sadržaj sadrži potrebne informacije okidač na DLP pravila kada je procijeniti.</span><span class="sxs-lookup"><span data-stu-id="945d4-103">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="945d4-104">Ako, na primjer, za **kreditne kartice pravila** konfiguriran s razinu pouzdanosti 85%, sljedeće vrednuju i morate otkrio za pravilo okidač:</span><span class="sxs-lookup"><span data-stu-id="945d4-104">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="945d4-105">**[Oblik:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 znamenki koje možete oblikovani ili neoblikovani (dddddddddddddddd) i mora proći Luhn test.</span><span class="sxs-lookup"><span data-stu-id="945d4-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="945d4-106">**[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Vrlo složene i robustan uzorak koji otkrije karte iz svih glavna gnojiva svijetu, uključujući Visa, Mastercard, otkrivanje kartica, JCB, American Express, poklon, i diner kartice.</span><span class="sxs-lookup"><span data-stu-id="945d4-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="945d4-107">**[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Da, Luhn kontrolni zbroj</span><span class="sxs-lookup"><span data-stu-id="945d4-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="945d4-108">**[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP pravila je % 85 sigurni da je otkrio ovu vrstu osjetljive informacije ako unutar blizine 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="945d4-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="945d4-109">Funkcija Func_credit_card pronalazi sadržaja koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="945d4-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="945d4-110">Vrijedi nešto od sljedećeg:</span><span class="sxs-lookup"><span data-stu-id="945d4-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="945d4-111">Ključne riječi iz Keyword_cc_verification nije pronađen.</span><span class="sxs-lookup"><span data-stu-id="945d4-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="945d4-112">Pronađen ključne riječi iz Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="945d4-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="945d4-113">Funkcija Func_expiration_date pronalazi datum u obliku datuma desno.</span><span class="sxs-lookup"><span data-stu-id="945d4-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="945d4-114">Kontrolni zbroj prolaza</span><span class="sxs-lookup"><span data-stu-id="945d4-114">The checksum passes</span></span>
    
    <span data-ttu-id="945d4-115">Na primjer, sljedeći uzorak 'D okidač za DLP pravila broj kreditne kartice:</span><span class="sxs-lookup"><span data-stu-id="945d4-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="945d4-116">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="945d4-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="945d4-117">Istječe: 2/2009</span><span class="sxs-lookup"><span data-stu-id="945d4-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="945d4-118">Dodatne informacije na što je potreban **Broj kreditne kartice** otkrio za sadržaj potražite u sljedećoj sekciji ovog članka: [Što u osjetljive informacije vrste potražite kreditne kartice #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="945d4-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="945d4-119">Pomoću različitih osjetljivih informacija za ugrađene vrste, pogledajte sljedeći članak informacije na što je potrebno za druge vrste: [što u osjetljive informacije vrste Potraži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="945d4-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

