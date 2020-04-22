---
title: DLP pravilo za SAD / UK Passport Number ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 9d9615eccd1e245bf4ca32742bfc64321dd7a8cf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714978"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="af782-102">Problemi s DLP - US / UK brojeve putovnica</span><span class="sxs-lookup"><span data-stu-id="af782-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="af782-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="af782-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="af782-104">**DLP pitanja s američkim / UK brojevima putovnica**</span><span class="sxs-lookup"><span data-stu-id="af782-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="af782-105">Imate li problema s **a Data Loss Prevention (DLP)** ne radi za sadržaj koji sadrži broj **putovnice SAD-a/UK** kada koristite dlp osjetljivu vrstu informacija u sustavu O365?</span><span class="sxs-lookup"><span data-stu-id="af782-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="af782-106">Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije za ono što DLP pravila traže prilikom procjene.</span><span class="sxs-lookup"><span data-stu-id="af782-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="af782-107">Na primjer, za pravilo **broja broja putovnica SAD-a/Ujedinjene Kraljevine** konfigurirane s razinom pouzdanosti od 75 %, ocjenjuju se sljedeće i moraju se otkriti kako bi se pravilo pokrenulo</span><span class="sxs-lookup"><span data-stu-id="af782-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="af782-108">**[Oblik zapisa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devet znamenki</span><span class="sxs-lookup"><span data-stu-id="af782-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="af782-109">**[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devet uzastopnih znamenki</span><span class="sxs-lookup"><span data-stu-id="af782-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="af782-110">**[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nema šah-suma.</span><span class="sxs-lookup"><span data-stu-id="af782-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="af782-111">**[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika je 75% uvjeren da je otkrio ovu vrstu osjetljivih informacija ako, u blizini 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="af782-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="af782-112">Funkcija Func_usa_uk_passport pronalazi sadržaj koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="af782-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="af782-113">Ključna riječ iz Keyword_passport je pronađena.</span><span class="sxs-lookup"><span data-stu-id="af782-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="af782-114">Na primjer, sljedeći uzorak aktivirao bi se za pravilnik o **broju putovnica SAD-a i Ujedinjene Kraljevine:** Broj putovnice SAD-a 123456789</span><span class="sxs-lookup"><span data-stu-id="af782-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="af782-115">Dodatne informacije o tome što je potrebno za otkrivenje broja putovnice u SAD-u/UK za vaš sadržaj potražite u sljedećem odjeljku: [Što vrste osjetljivih informacija traže broj putovnice u SAD-u/Uk-u](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="af782-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="af782-116">Pomoću druge ugrađene osjetljive vrste informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [Što zahtijevaju osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="af782-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  