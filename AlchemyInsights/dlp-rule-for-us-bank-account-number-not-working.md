---
title: DLP pravilo za broj američkog bankovnog računa ne radi
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
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977154"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="6a9b9-102">DLP problemi s američkim brojevima bankovnih računa</span><span class="sxs-lookup"><span data-stu-id="6a9b9-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="6a9b9-103">**Važno**: Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i onedrive ostanu vrlo dostupne – dodatne informacije [potražite u članku Prilagodbe privremenih značajki sustava SharePoint Online.](https://aka.ms/ODSPAdjustments)</span><span class="sxs-lookup"><span data-stu-id="6a9b9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="6a9b9-104">**DLP problemi s američkim brojevima bankovnih računa**</span><span class="sxs-lookup"><span data-stu-id="6a9b9-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="6a9b9-105">Imate li problema s **a Data Loss Prevention (DLP)** ne radi za sadržaj koji sadrži broj računa **američke banke** kada koristite DLP osjetljive vrste informacija u O365?</span><span class="sxs-lookup"><span data-stu-id="6a9b9-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="6a9b9-106">Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije za ono što DLP pravila traže prilikom procjene.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="6a9b9-107">Na primjer, za pravilnik **o broju bankovnog računa SAD-a** konfiguriranog s razinom pouzdanosti od 85 %, vrednuju se sljedeće i mora se otkriti da bi se pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="6a9b9-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="6a9b9-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 znamenki</span><span class="sxs-lookup"><span data-stu-id="6a9b9-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="6a9b9-109">**[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 uzastopnih znamenki.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="6a9b9-110">**[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nema šah-suma.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="6a9b9-111">**[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP politika je 75% uvjeren da je otkrio ovu vrstu osjetljivih informacija ako, u blizini 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="6a9b9-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="6a9b9-112">Regularni izraz Regex_usa_bank_account_number pronalazi sadržaj koji odgovara uzorku</span><span class="sxs-lookup"><span data-stu-id="6a9b9-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="6a9b9-113">Ključna riječ iz Keyword_usa_Bank_Account je pronađena.</span><span class="sxs-lookup"><span data-stu-id="6a9b9-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="6a9b9-114">Na primjer, sljedeći uzorak će se pokrenuti za **pravilnik o broju bankovnog računa SAD-a:** Tekući račun 78344011</span><span class="sxs-lookup"><span data-stu-id="6a9b9-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="6a9b9-115">Dodatne informacije o tome što je potrebno za detektiranje broja bankovnog računa u **SAD-u** za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže broj bankovnog računa u SAD-u](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="6a9b9-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="6a9b9-116">Pomoću druge ugrađene osjetljive vrste informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [Što zahtijevaju osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="6a9b9-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  