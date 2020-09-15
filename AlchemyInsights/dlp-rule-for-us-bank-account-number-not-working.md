---
title: DLP pravilo za broj bankovnog računa za US ne funkcionira
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679288"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="df06a-102">DLP problemi s brojevima bankovnog računa za US</span><span class="sxs-lookup"><span data-stu-id="df06a-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="df06a-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="df06a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="df06a-104">**DLP problemi s brojevima bankovnog računa za US**</span><span class="sxs-lookup"><span data-stu-id="df06a-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="df06a-105">Imate li problema s **prevencijom gubitka podataka (DLP)** ne radi za sadržaj koji sadrži **broj bankovnog računa za US** kada koristite DLP osjetljivu vrstu podataka u programu O365?</span><span class="sxs-lookup"><span data-stu-id="df06a-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="df06a-106">Ako je tako, provjerite sadrži li sadržaj potrebne informacije o tome što pravilnik programa DLP traži kada se procjenjuje.</span><span class="sxs-lookup"><span data-stu-id="df06a-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="df06a-107">Primjerice, za pravila **broja bankovnog računa za US** koja je konfigurirana uz razinu pouzdanosti od 85%, procjenjuje se sljedeće i mora se otkriti da bi se pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="df06a-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="df06a-108">**[Oblikovanje:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 znamenaka</span><span class="sxs-lookup"><span data-stu-id="df06a-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="df06a-109">**[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 uzastopnih znamenki.</span><span class="sxs-lookup"><span data-stu-id="df06a-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="df06a-110">**[Potvrdni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ne postoji checksum</span><span class="sxs-lookup"><span data-stu-id="df06a-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="df06a-111">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP pravilo je 75% pouzdano da je otkrivena ta vrsta osjetljivih podataka ako je u neposrednoj blizini znakova od 300:</span><span class="sxs-lookup"><span data-stu-id="df06a-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="df06a-112">Uobičajeni izraz Regex_usa_bank_account_number pronalazi sadržaj koji odgovara uzorku</span><span class="sxs-lookup"><span data-stu-id="df06a-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="df06a-113">Pronađena je ključna riječ iz Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="df06a-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="df06a-114">Na primjer, sljedeći će se uzorak pokrenuti za pravilnik o **broju bankovnog računa u sad** -u: tekući račun 78344011</span><span class="sxs-lookup"><span data-stu-id="df06a-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="df06a-115">Dodatne informacije o tome što je potrebno za **broj bankovnog računa za US** da bi se otkrilo za sadržaj potražite u sljedećem odjeljku u ovom članku: [što vrste osjetljivih podataka traže broj bankovnog računa za nas](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="df06a-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="df06a-116">Korištenje različitih ugrađenih vrsta osjetljivih informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [što vrste osjetljivih podataka traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="df06a-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  