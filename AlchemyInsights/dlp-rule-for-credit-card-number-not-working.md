---
title: DLP pravilo za broj kreditne kartice ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932435"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="b0748-102">DLP problemi s brojevima kreditnih kartica</span><span class="sxs-lookup"><span data-stu-id="b0748-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="b0748-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="b0748-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b0748-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="b0748-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b0748-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="b0748-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b0748-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="b0748-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b0748-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="b0748-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b0748-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="b0748-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b0748-109">**DLP problemi s brojevima kreditnih kartica**</span><span class="sxs-lookup"><span data-stu-id="b0748-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="b0748-110">Imate li problema s **sprječavanjem gubitka podataka (DLP)** koji ne radi za sadržaj koji sadrži **broj kreditne kartice** kada koristite vrstu podataka osjetljivih na DLP u sustavu O365?</span><span class="sxs-lookup"><span data-stu-id="b0748-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="b0748-111">Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije za pokretanje pravila DLP-a prilikom procjene.</span><span class="sxs-lookup"><span data-stu-id="b0748-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="b0748-112">Na primjer, za **pravila kreditne kartice** konfigurirane s razinom pouzdanosti od 85%, vrednuju se sljedeće i mora se otkriti da bi se pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="b0748-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="b0748-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 znamenki koje se mogu formatirati ili neformatirati (ddddddddddddddd) i moraju proći Luhn test.</span><span class="sxs-lookup"><span data-stu-id="b0748-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="b0748-114">**[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Vrlo složen i robustan uzorak koji otkriva kartice iz svih glavnih marki širom svijeta, uključujući Visa, MasterCard, Discover Card, JCB, American Express, poklon kartice, i diner kartice.</span><span class="sxs-lookup"><span data-stu-id="b0748-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="b0748-115">**[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Da, Luhn kontrolni zbroj.</span><span class="sxs-lookup"><span data-stu-id="b0748-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="b0748-116">**[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politika je 85% uvjeren da je otkrio ovu vrstu osjetljivih informacija ako, u blizini 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="b0748-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="b0748-117">Funkcija Func_credit_card pronalazi sadržaj koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="b0748-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="b0748-118">Točno je jedno od sljedećeg:</span><span class="sxs-lookup"><span data-stu-id="b0748-118">One of the following is true:</span></span>

  - <span data-ttu-id="b0748-119">Ključna riječ iz Keyword_cc_verification je pronađena.</span><span class="sxs-lookup"><span data-stu-id="b0748-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="b0748-120">Ključna riječ iz Keyword_cc_name je pronađena</span><span class="sxs-lookup"><span data-stu-id="b0748-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="b0748-121">Funkcija Func_expiration_date pronalazi datum u pravom obliku datuma.</span><span class="sxs-lookup"><span data-stu-id="b0748-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="b0748-122">Kontrolni zbroj prolazi</span><span class="sxs-lookup"><span data-stu-id="b0748-122">The checksum passes</span></span>

    <span data-ttu-id="b0748-123">Na primjer, sljedeći uzorak će se pokrenuti za DLP Credit Card Number Policy:</span><span class="sxs-lookup"><span data-stu-id="b0748-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="b0748-124">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="b0748-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="b0748-125">Ističe: 2/2009</span><span class="sxs-lookup"><span data-stu-id="b0748-125">Expires: 2/2009</span></span>

<span data-ttu-id="b0748-126">Dodatne informacije o tome što je potrebno za detektiranje **broja kreditne kartice** za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže kreditnu karticu#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="b0748-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="b0748-127">Pomoću druge ugrađene osjetljive vrste informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [Što zahtijevaju osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="b0748-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  