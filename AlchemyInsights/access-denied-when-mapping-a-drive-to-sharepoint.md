---
title: Pristup odbijen prilikom mapiranja pogona SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737469"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="5af98-102">Riješite probleme sa SharePoint biblioteke mapirani mrežni pogoni</span><span class="sxs-lookup"><span data-stu-id="5af98-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="5af98-103">Prilikom pregledavanja preslikan mrežni pogon, može se pojaviti jedna od sljedećih poruka:</span><span class="sxs-lookup"><span data-stu-id="5af98-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="5af98-104">**\\Put se ne može pristupiti. Možda nemate dozvolu za korištenje tog mrežnog resursa. Obratite se administratoru poslužitelja da biste saznali imate dozvole pristupa.**</span><span class="sxs-lookup"><span data-stu-id="5af98-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="5af98-105">**Pristup je odbijen. Prije otvaranja datoteka na ovom mjestu morate prvo dodajte web-mjesta na popis pouzdanih web-mjesta, pregledajte web-mjesto i odaberite mogućnost za automatsku prijavu.**</span><span class="sxs-lookup"><span data-stu-id="5af98-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="5af98-106">[Otklanjanje poteškoća pomoći Dohvati preslikane mrežne pogone](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="5af98-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="5af98-107">Mapiranje biblioteku kao mrežni pogon je privremena i podržani samo u programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="5af98-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="5af98-108">Umjesto toga, [sinkronizirati datoteke SharePoint s novom klijentu sinkronizaciju OneDrive](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) koji uključuje [Datoteke na zahtjev](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="5af98-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="5af98-109">Sve datoteke u OneDrive pristupiti bez korištenja lokalnog prostora.</span><span class="sxs-lookup"><span data-stu-id="5af98-109">Access all your files in OneDrive without using local storage space.</span></span>
  