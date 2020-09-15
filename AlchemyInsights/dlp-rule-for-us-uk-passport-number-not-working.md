---
title: DLP pravilo za nas/broj putovnica u Velikoj Britaniji ne funkcionira
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679216"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="5b171-102">Problemi s brojem putovnica za DLP-US/UK</span><span class="sxs-lookup"><span data-stu-id="5b171-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="5b171-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="5b171-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5b171-104">**DLP problemi s brojem putovnica za US/UK**</span><span class="sxs-lookup"><span data-stu-id="5b171-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="5b171-105">Imate li problema s **prevencijom gubitka podataka (DLP)** koji ne funkcionira za sadržaj koji sadrži **broj putovnice za US/UK** kada koristite DLP osjetljive informacije u programu O365?</span><span class="sxs-lookup"><span data-stu-id="5b171-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="5b171-106">Ako je tako, provjerite sadrži li sadržaj potrebne informacije o tome što pravilnik programa DLP traži kada se procjenjuje.</span><span class="sxs-lookup"><span data-stu-id="5b171-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="5b171-107">Primjerice, za pravilnik o **broju putovnica za US/UK** konfiguriran uz razinu pouzdanosti od 75%, procjenjuje se sljedeće i mora se otkriti da bi se pravilo pokrenulo</span><span class="sxs-lookup"><span data-stu-id="5b171-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="5b171-108">**[Oblikovanje:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet znamenki</span><span class="sxs-lookup"><span data-stu-id="5b171-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="5b171-109">**[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet uzastopnih znamenki</span><span class="sxs-lookup"><span data-stu-id="5b171-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="5b171-110">**[Potvrdni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ne postoji checksum</span><span class="sxs-lookup"><span data-stu-id="5b171-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="5b171-111">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP pravilo je 75% pouzdano da je otkrivena ta vrsta osjetljivih podataka ako je u neposrednoj blizini znakova od 300:</span><span class="sxs-lookup"><span data-stu-id="5b171-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="5b171-112">Funkcija Func_usa_uk_passport pronalazi sadržaj koji odgovara uzorku.</span><span class="sxs-lookup"><span data-stu-id="5b171-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="5b171-113">Pronađena je ključna riječ iz Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="5b171-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="5b171-114">Primjerice, sljedeći će se uzorak pokrenuti za pravilnik o **broju putovnica Sjedinjenih Američkih Država/UK** : Američka putovnica broj 123456789</span><span class="sxs-lookup"><span data-stu-id="5b171-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="5b171-115">Dodatne informacije o tome što je potrebno za broj putovnica za US/UK da bi se otkrilo za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [što vrste osjetljivih informacija traže nas/broj putovnica Britanije](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="5b171-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="5b171-116">Korištenje različitih ugrađenih vrsta osjetljivih informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [što vrste osjetljivih podataka traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="5b171-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  