---
title: DLP pravilo za broj kreditne kartice ne funkcionira
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679433"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="33559-102">DLP problemi s brojevima kreditnih kartica</span><span class="sxs-lookup"><span data-stu-id="33559-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="33559-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="33559-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="33559-104">**DLP problemi s brojevima kreditnih kartica**</span><span class="sxs-lookup"><span data-stu-id="33559-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="33559-105">Imate li problema s **prevencijom gubitka podataka (DLP)** ne radi za sadržaj koji sadrži **broj kreditne kartice** kada koristite DLP osjetljive informacije u O365?</span><span class="sxs-lookup"><span data-stu-id="33559-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="33559-106">Ako je tako, provjerite sadrži li sadržaj potrebne informacije da biste pokrenuli pravilnik programa DLP kada se procjenjuje.</span><span class="sxs-lookup"><span data-stu-id="33559-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="33559-107">Primjerice, ako je **pravilnik o kreditnoj kartici** konfiguriran s razinom pouzdanosti od 85%, procjenjuje se sljedeće i mora se otkriti da bi se pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="33559-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="33559-108">**[Oblik:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 znamenaka koje je moguće formatirati ili neoblikovati (dddddddddddddddde) i mora proći kroz Luhn test.</span><span class="sxs-lookup"><span data-stu-id="33559-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="33559-109">**[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Vrlo složen i robustan uzorak koji detektira kartice svih glavnih marki diljem svijeta, uključujući vizu, MasterCard, Discover Card, JCB, American Express, poklon-bonove i kartice Diner.</span><span class="sxs-lookup"><span data-stu-id="33559-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="33559-110">**[Potvrdni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, Luhn ček</span><span class="sxs-lookup"><span data-stu-id="33559-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="33559-111">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP pravilo je 85% pouzdano da je otkrivena ta vrsta osjetljivih podataka ako je u neposrednoj blizini znakova od 300:</span><span class="sxs-lookup"><span data-stu-id="33559-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="33559-112">Funkcija Func_credit_card pronalazi sadržaj koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="33559-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="33559-113">Vrijedi jedno od sljedećeg:</span><span class="sxs-lookup"><span data-stu-id="33559-113">One of the following is true:</span></span>

  - <span data-ttu-id="33559-114">Pronađena je ključna riječ iz Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="33559-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="33559-115">Pronađena je ključna riječ iz Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="33559-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="33559-116">Funkcija Func_expiration_date pronalazi Datum u pravom obliku datuma.</span><span class="sxs-lookup"><span data-stu-id="33559-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="33559-117">Potvrdni zbroj prolazi</span><span class="sxs-lookup"><span data-stu-id="33559-117">The checksum passes</span></span>

    <span data-ttu-id="33559-118">Na primjer, sljedeći uzorak potaknuti će pravilnik o broju kartica za DLP:</span><span class="sxs-lookup"><span data-stu-id="33559-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="33559-119">Viza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="33559-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="33559-120">Istječe: 2/2009</span><span class="sxs-lookup"><span data-stu-id="33559-120">Expires: 2/2009</span></span>

<span data-ttu-id="33559-121">Dodatne informacije o potrebi otkrivanja **broja kreditnih kartica** za sadržaj potražite u sljedećem odjeljku u ovom članku: [što vrste osjetljivih informacija traže kreditnu karticu #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="33559-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="33559-122">Korištenje različitih ugrađenih vrsta osjetljivih informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [što vrste osjetljivih podataka traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="33559-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  