---
title: O sigurnosnim ažuriranjima sustava Exchange Server
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481119"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="88670-102">O sigurnosnim ažuriranjima sustava Exchange Server</span><span class="sxs-lookup"><span data-stu-id="88670-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="88670-103">Microsoft je objavio niz kritičnih sigurnosnih ažuriranja za lokalno Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="88670-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="88670-104">Primijenjenih poslužitelja verzije su bilo koje ažuriranje razina sustava Exchange Server 2010, 2013, 2016 i 2019.</span><span class="sxs-lookup"><span data-stu-id="88670-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="88670-105">Exchange Online nije utjecao, ali ako imate neke lokalne poslužitelje sustava Exchange zbog hibridne konfiguracije, potencijalno su ranjivi.</span><span class="sxs-lookup"><span data-stu-id="88670-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="88670-106">Da biste ažurirali lokalne poslužitelje, morat ćete pokrenuti najmanje sljedeće verzije sustava Exchange:</span><span class="sxs-lookup"><span data-stu-id="88670-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="88670-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="88670-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="88670-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="88670-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="88670-109">Exchange Server 2016 CU 19 ili CU 18</span><span class="sxs-lookup"><span data-stu-id="88670-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="88670-110">Exchange Server 2019 CU 8 ili CU 7</span><span class="sxs-lookup"><span data-stu-id="88670-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="88670-111">Pročitajte sljedeće priopćenje za mjesto popravaka: [Objavljeno: ožujak 2021 Exchange Server Security Update](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="88670-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="88670-112">**Važne napomene:**</span><span class="sxs-lookup"><span data-stu-id="88670-112">**Important notes:**</span></span>

<span data-ttu-id="88670-113">Instalacija ažuriranja neće funkcionirati ako lokalni poslužitelji ne pokrenu potrebne verzije sustava Exchange, kao na gornjem popisu.</span><span class="sxs-lookup"><span data-stu-id="88670-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="88670-114">Ako instalirate ažuriranja ručno, pročitajte odjeljak "poznati problemi" za članke iz servisa Update KB za važne informacije.</span><span class="sxs-lookup"><span data-stu-id="88670-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="88670-115">Sigurnosno se ažuriranje mora pokrenuti s povišenim CMD/PowerShell upita!</span><span class="sxs-lookup"><span data-stu-id="88670-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
