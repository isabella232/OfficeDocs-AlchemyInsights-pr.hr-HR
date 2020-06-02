---
title: DLP pravilo za američki broj bankovnog računa ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507326"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="23e3b-102">DLP problemi s američkim brojevima bankovnih računa</span><span class="sxs-lookup"><span data-stu-id="23e3b-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="23e3b-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="23e3b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="23e3b-104">**DLP problemi s američkim brojevima bankovnih računa**</span><span class="sxs-lookup"><span data-stu-id="23e3b-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="23e3b-105">Imate li problema s **sprječavanjem gubitka podataka (DLP)** koji ne radi za sadržaj koji sadrži **broj bankovnog računa SAD-a** kada koristite vrstu osjetljivih informacija o DLP-u u sustavu O365?</span><span class="sxs-lookup"><span data-stu-id="23e3b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="23e3b-106">Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije o tome što pravila DLP-a traže kada se ocjenjuju.</span><span class="sxs-lookup"><span data-stu-id="23e3b-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="23e3b-107">Na primjer, za pravilo **broja bankovnog računa SAD-a** konfigurirano s razinom pouzdanosti od 85%, ocjenjuju se sljedeće i moraju se otkriti da bi se pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="23e3b-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="23e3b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 znamenki</span><span class="sxs-lookup"><span data-stu-id="23e3b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="23e3b-109">**[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 uzastopnih znamenki.</span><span class="sxs-lookup"><span data-stu-id="23e3b-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="23e3b-110">**[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nema Kontrolnog zbroja.</span><span class="sxs-lookup"><span data-stu-id="23e3b-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="23e3b-111">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP politika je 75% sigurni da je otkrivena ova vrsta osjetljivih informacija ako, u blizini od 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="23e3b-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="23e3b-112">Regularni izraz Regex_usa_bank_account_number pronalazi sadržaj koji odgovara uzorku</span><span class="sxs-lookup"><span data-stu-id="23e3b-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="23e3b-113">Ključna riječ iz Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="23e3b-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="23e3b-114">Na primjer, sljedeći uzorak pokrenuo bi se za pravila **broja bankovnog računa SAD-a:** Tekući račun 78344011</span><span class="sxs-lookup"><span data-stu-id="23e3b-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="23e3b-115">Dodatne informacije o tome što je potrebno za **otkriveni broj bankovnog računa SAD-a** za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže broj američkog bankovnog računa](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="23e3b-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="23e3b-116">Pomoću druge ugrađene vrste osjetljivih informacija pogledajte sljedeći članak za informacije o tome što je potrebno za druge vrste: [Što traže vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="23e3b-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  