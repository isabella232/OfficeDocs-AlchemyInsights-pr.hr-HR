---
title: DLP Policy Savjeti ne rade
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932578"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="e5945-102">DLP Politika Savjet pitanja</span><span class="sxs-lookup"><span data-stu-id="e5945-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="e5945-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="e5945-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e5945-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="e5945-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e5945-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="e5945-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e5945-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="e5945-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e5945-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="e5945-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e5945-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="e5945-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e5945-109">**DLP policy savjeti**</span><span class="sxs-lookup"><span data-stu-id="e5945-109">**DLP policy tips**</span></span>

<span data-ttu-id="e5945-110">Prilikom korištenja **DLP pravila**korisnici mogu biti obaviješteni o kršenju pravila s **savjetima o pravilima**.</span><span class="sxs-lookup"><span data-stu-id="e5945-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="e5945-111">Administratori mogu konfigurirati savjete o pravilima za prikaz tijekom testiranja pravila dlp-a ili kada je pravilo u punom načinu izvršavanja.</span><span class="sxs-lookup"><span data-stu-id="e5945-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="e5945-112">Da biste u punom načinu izvršavanja konfigurirali savjete o pravilima pravila za pravila pravila o pravilima za pravila o sigurnosti i usklađenosti, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="e5945-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="e5945-113">Provjerite jesu li na pravilu **omogućeni** savjeti za pravila za Pravilo DLP-a pomoću [koraka ovdje](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="e5945-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="e5945-114">Provjerite **odgovara** li vaš sadržaj onome što je **potrebno** za pokretanje pravila navedenog u ovom članku [ovdje](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="e5945-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="e5945-115">Savjeti za pravila prikazuju se u programima OWA i outlook.</span><span class="sxs-lookup"><span data-stu-id="e5945-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="e5945-116">Međutim, kada koristite **Outlook 2013 ili noviji,** savjeti za pravila prikazuju se samo pod određenim uvjetima.</span><span class="sxs-lookup"><span data-stu-id="e5945-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="e5945-117">Ovi su uvjeti navedeni ovdje: [Podržani uvjeti za Outlook 2013 ili noviji za prikaz savjeta o pravilima](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="e5945-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="e5945-118">Dodatne informacije o savjetima o Pravilima dlp-a potražite u odjeljku Prikaz [savjeta o pravilima za DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="e5945-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  