---
title: DLP pravilo za nas broj bankovnog računa ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529851"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="d6700-102">DLP problemi s NAMA brojeve bankovnih računa</span><span class="sxs-lookup"><span data-stu-id="d6700-102">DLP issues with US Bank Account Numbers</span></span>

<span data-ttu-id="d6700-103">Imate li problema s **Podataka gubitak Data Execution Prevention (DLP)** ne rade za sadržaj koji sadrži **Broj bankovnog računa sad** kada koristite vrstu osjetljive informacije DLP u O365?</span><span class="sxs-lookup"><span data-stu-id="d6700-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d6700-104">Ako je tako, provjerite je li vaš sadržaj sadrži potrebne informacije za što je tražite pravila DLP prilikom procjene.</span><span class="sxs-lookup"><span data-stu-id="d6700-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d6700-105">Ako, na primjer, za **Broj bankovnog računa za AMERIČKI** pravila konfiguriran s razinu pouzdanosti 85%, sljedeće vrednuju i morate otkrio za pravilo okidač:</span><span class="sxs-lookup"><span data-stu-id="d6700-105">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d6700-106">**[Obliku:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8 17 znamenki</span><span class="sxs-lookup"><span data-stu-id="d6700-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="d6700-107">**[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8 17 uzastopne znamenki.</span><span class="sxs-lookup"><span data-stu-id="d6700-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="d6700-108">**[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne postoji nijedan kontrolni zbroj</span><span class="sxs-lookup"><span data-stu-id="d6700-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d6700-109">**[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Pravila DLP je 75% sigurni da je otkrio ovu vrstu osjetljive informacije ako unutar blizine 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="d6700-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d6700-110">Regularni izraz Regex_usa_bank_account_number pronalazi sadržaja koji odgovara uzorku</span><span class="sxs-lookup"><span data-stu-id="d6700-110">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="d6700-111">Ključne riječi iz Keyword_usa_Bank_Account nije pronađen.</span><span class="sxs-lookup"><span data-stu-id="d6700-111">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="d6700-112">Ako, na primjer, sljedeći uzorak 'D okidač za pravila **Sad broj bankovnog računa** : Provjera računa 78344011</span><span class="sxs-lookup"><span data-stu-id="d6700-112">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="d6700-113">Dodatne informacije na što je potrebno za **AMERIČKI broj bankovnog računa** za otkrio za sadržaj potražite u sljedećoj sekciji ovog članka: [Što u osjetljive informacije vrste potražite broj bankovnog računa za SAD](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="d6700-113">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="d6700-114">Pomoću različitih osjetljivih informacija za ugrađene vrste, pogledajte sljedeći članak informacije na što je potrebno za druge vrste: [što u osjetljive informacije vrste Potraži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d6700-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  