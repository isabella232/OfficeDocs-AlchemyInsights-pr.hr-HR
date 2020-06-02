---
title: DLP pravilo za američki/britanski broj putovnice ne radi
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
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507290"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="e2fea-102">Problemi s DLP - Američki /Britanski brojevi putovnica</span><span class="sxs-lookup"><span data-stu-id="e2fea-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="e2fea-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="e2fea-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="e2fea-104">**DLP problemi s američkim /britanskim brojevima putovnica**</span><span class="sxs-lookup"><span data-stu-id="e2fea-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="e2fea-105">Imate li problema s **Sprječavanje gubitka podataka (DLP)** ne radi za sadržaj koji sadrži **američki / UK broj putovnice** kada koristite DLP osjetljive vrste informacija u O365?</span><span class="sxs-lookup"><span data-stu-id="e2fea-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="e2fea-106">Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije o tome što pravila DLP-a traže kada se ocjenjuju.</span><span class="sxs-lookup"><span data-stu-id="e2fea-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="e2fea-107">Na primjer, za politiku **broja putovnica SAD-a/Ujedinjene Kraljevine** konfigurirana s razinom pouzdanosti od 75 %, ocjenjuju se sljedeće i moraju se otkriti kako bi pravilo pokrenulo</span><span class="sxs-lookup"><span data-stu-id="e2fea-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="e2fea-108">**[Oblik:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet znamenki</span><span class="sxs-lookup"><span data-stu-id="e2fea-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="e2fea-109">**[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet uzastopnih znamenki</span><span class="sxs-lookup"><span data-stu-id="e2fea-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="e2fea-110">**[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nema Kontrolnog zbroja.</span><span class="sxs-lookup"><span data-stu-id="e2fea-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="e2fea-111">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP politika je 75% sigurni da je otkrivena ova vrsta osjetljivih informacija ako, u blizini od 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="e2fea-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="e2fea-112">Funkcija Func_usa_uk_passport pronalazi sadržaj koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="e2fea-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="e2fea-113">Ključna riječ iz Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="e2fea-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="e2fea-114">Na primjer, sljedeći uzorak pokrenuo bi se za politiku **broja putovnice SAD-a/Ujedinjene Kraljevine:** Američki broj putovnice 123456789</span><span class="sxs-lookup"><span data-stu-id="e2fea-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="e2fea-115">Dodatne informacije o tome što je potrebno za otkriveni broj putovnice u SAD-u/UK-u za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže broj putovnice SAD-a i Velike Britanije](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="e2fea-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="e2fea-116">Pomoću druge ugrađene vrste osjetljivih informacija pogledajte sljedeći članak za informacije o tome što je potrebno za druge vrste: [Što traže vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="e2fea-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  