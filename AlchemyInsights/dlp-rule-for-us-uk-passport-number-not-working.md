---
title: DLP pravilo za SAD / UK Passport Number ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931254"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="864a1-102">Problemi s DLP - US / UK brojeve putovnica</span><span class="sxs-lookup"><span data-stu-id="864a1-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="864a1-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="864a1-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="864a1-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="864a1-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="864a1-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="864a1-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="864a1-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="864a1-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="864a1-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="864a1-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="864a1-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="864a1-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="864a1-109">**DLP pitanja s američkim / UK brojevima putovnica**</span><span class="sxs-lookup"><span data-stu-id="864a1-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="864a1-110">Imate li problema s **a Data Loss Prevention (DLP)** ne radi za sadržaj koji sadrži broj **putovnice SAD-a/UK** kada koristite dlp osjetljivu vrstu informacija u sustavu O365?</span><span class="sxs-lookup"><span data-stu-id="864a1-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="864a1-111">Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije za ono što DLP pravila traže prilikom procjene.</span><span class="sxs-lookup"><span data-stu-id="864a1-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="864a1-112">Na primjer, za pravilo **broja broja putovnica SAD-a/Ujedinjene Kraljevine** konfigurirane s razinom pouzdanosti od 75 %, ocjenjuju se sljedeće i moraju se otkriti kako bi se pravilo pokrenulo</span><span class="sxs-lookup"><span data-stu-id="864a1-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="864a1-113">**[Oblik zapisa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devet znamenki</span><span class="sxs-lookup"><span data-stu-id="864a1-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="864a1-114">**[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devet uzastopnih znamenki</span><span class="sxs-lookup"><span data-stu-id="864a1-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="864a1-115">**[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nema šah-suma.</span><span class="sxs-lookup"><span data-stu-id="864a1-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="864a1-116">**[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika je 75% uvjeren da je otkrio ovu vrstu osjetljivih informacija ako, u blizini 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="864a1-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="864a1-117">Funkcija Func_usa_uk_passport pronalazi sadržaj koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="864a1-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="864a1-118">Ključna riječ iz Keyword_passport je pronađena.</span><span class="sxs-lookup"><span data-stu-id="864a1-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="864a1-119">Na primjer, sljedeći uzorak aktivirao bi se za pravilnik o **broju putovnica SAD-a i Ujedinjene Kraljevine:** Broj putovnice SAD-a 123456789</span><span class="sxs-lookup"><span data-stu-id="864a1-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="864a1-120">Dodatne informacije o tome što je potrebno za otkrivenje broja putovnice u SAD-u/UK za vaš sadržaj potražite u sljedećem odjeljku: [Što vrste osjetljivih informacija traže broj putovnice u SAD-u/Uk-u](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="864a1-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="864a1-121">Pomoću druge ugrađene osjetljive vrste informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [Što zahtijevaju osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="864a1-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  