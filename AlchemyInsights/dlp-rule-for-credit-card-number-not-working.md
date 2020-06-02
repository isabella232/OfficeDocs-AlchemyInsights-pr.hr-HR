---
title: DLP pravilo za broj kreditne kartice ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507398"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="bd399-102">DLP problemi s brojevima kreditnih kartica</span><span class="sxs-lookup"><span data-stu-id="bd399-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="bd399-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="bd399-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="bd399-104">**DLP problemi s brojevima kreditnih kartica**</span><span class="sxs-lookup"><span data-stu-id="bd399-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="bd399-105">Imate li problema s **sprječavanjem gubitka podataka (DLP)** koji ne radi za sadržaj koji sadrži **broj kreditne kartice** kada koristite DLP osjetljivu vrstu informacija u sustavu O365?</span><span class="sxs-lookup"><span data-stu-id="bd399-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="bd399-106">Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije da biste pokrenuli pravilo DLP-a prilikom procjene.</span><span class="sxs-lookup"><span data-stu-id="bd399-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="bd399-107">Na primjer, da bi **pravila kreditne kartice** konfigurirana s razinom pouzdanosti od 85%, ocjenjuju se sljedeće i moraju se otkriti da bi se pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="bd399-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="bd399-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 znamenki koje se mogu formatirati ili neformatirane (dddddddddddddd) i moraju proći Test Luhn.</span><span class="sxs-lookup"><span data-stu-id="bd399-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="bd399-109">**[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Vrlo složen i robustan uzorak koji otkriva kartice svih glavnih marki širom svijeta, uključujući Visa, MasterCard, Discover Card, JCB, American Express, poklon kartice i diner kartice.</span><span class="sxs-lookup"><span data-stu-id="bd399-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="bd399-110">**[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, Luhn checksum.</span><span class="sxs-lookup"><span data-stu-id="bd399-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="bd399-111">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP politika je 85% sigurni da je otkrivena ova vrsta osjetljivih informacija ako, u blizini od 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="bd399-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="bd399-112">Funkcija Func_credit_card pronalazi sadržaj koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="bd399-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="bd399-113">Jedno od sljedećeg je istina:</span><span class="sxs-lookup"><span data-stu-id="bd399-113">One of the following is true:</span></span>

  - <span data-ttu-id="bd399-114">Ključna riječ iz Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="bd399-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="bd399-115">Ključna riječ Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="bd399-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="bd399-116">Funkcija Func_expiration_date pronalazi datum u ispravnom obliku datuma.</span><span class="sxs-lookup"><span data-stu-id="bd399-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="bd399-117">Kontrolni zbroj prolazi</span><span class="sxs-lookup"><span data-stu-id="bd399-117">The checksum passes</span></span>

    <span data-ttu-id="bd399-118">Na primjer, sljedeći uzorak će se pokrenuti za DLP pravila broja kreditne kartice:</span><span class="sxs-lookup"><span data-stu-id="bd399-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="bd399-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="bd399-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="bd399-120">Ističe: 2/2009</span><span class="sxs-lookup"><span data-stu-id="bd399-120">Expires: 2/2009</span></span>

<span data-ttu-id="bd399-121">Dodatne informacije o tome što je potrebno za otkriven broj **kreditne kartice** za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže kreditnu karticu#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="bd399-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="bd399-122">Pomoću druge ugrađene vrste osjetljivih informacija pogledajte sljedeći članak za informacije o tome što je potrebno za druge vrste: [Što traže vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="bd399-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  