---
title: Pristup je odbijen prilikom mapiranja pogona u SharePoint
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737469"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="36336-102">Rješavanje problema s bibliotekama sustava SharePoint mapiranih na mrežne pogone</span><span class="sxs-lookup"><span data-stu-id="36336-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="36336-103">Kada pregledavate mapirani mrežni pogon, možda ćete vidjeti jednu od sljedećih poruka:</span><span class="sxs-lookup"><span data-stu-id="36336-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="36336-104">**\\Put nije dostupan. Možda nemate dozvolu za korištenje ovog mrežnog resursa. Obratite se administratoru ovog poslužitelja da biste saznali imate li dozvole za pristup.**</span><span class="sxs-lookup"><span data-stu-id="36336-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="36336-105">**Pristup odbijen. Prije otvaranja datoteka na ovom mjestu, najprije morate dodati web-mjesto na svoj popis pouzdanog web-mjesta, potražiti web-mjesto i odabrati mogućnost automatskog prijave.**</span><span class="sxs-lookup"><span data-stu-id="36336-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="36336-106">[Nabavite pomoć za otklanjanje poteškoća s mapiranih mrežnih pogona](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="36336-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="36336-107">Mapiranje biblioteke kao mrežnog pogona privremeno je i podržano samo u pregledniku Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="36336-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="36336-108">Umjesto toga, [Sinkronizirajte SharePoint datoteke s novim klijentskim sinkronizacijom servisa OneDrive](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) koji uključuje [datoteke na zahtjev](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="36336-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="36336-109">Pristupite svim datotekama na servisu OneDrive bez korištenja lokalnog prostora za pohranu.</span><span class="sxs-lookup"><span data-stu-id="36336-109">Access all your files in OneDrive without using local storage space.</span></span>
  