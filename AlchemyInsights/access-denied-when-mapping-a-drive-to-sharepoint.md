---
title: Pristup je odbijen prilikom mapiranja pogona u SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668735"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="3057f-102">Otklanjanje poteškoća s bibliotekama sustava SharePoint mapiranim na mrežne pogone</span><span class="sxs-lookup"><span data-stu-id="3057f-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="3057f-103">Kada otvorite mapirani mrežni pogon, možda ćete vidjeti neku od sljedećih poruka:</span><span class="sxs-lookup"><span data-stu-id="3057f-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="3057f-104">**\\Put nije pristupačan. Možda nemate dozvolu za korištenje tog mrežnog resursa. Obratite se administratoru ovog poslužitelja da biste saznali imate li dozvole za pristup.**</span><span class="sxs-lookup"><span data-stu-id="3057f-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="3057f-105">**Pristup je odbijen. Prije otvaranja datoteka na tom mjestu, najprije morate dodati web-mjesto na popis pouzdanih web-mjesta, potražiti web-mjesto i odabrati mogućnost automatskog prijave.**</span><span class="sxs-lookup"><span data-stu-id="3057f-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="3057f-106">[Pomoć za otklanjanje poteškoća s mapiranim mrežnim pogonima](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)</span><span class="sxs-lookup"><span data-stu-id="3057f-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="3057f-107">Mapiranje biblioteke kao mrežnog pogona privremeno je i podržano samo u pregledniku Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="3057f-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="3057f-108">Umjesto toga [sinkronizirajte datoteke sustava SharePoint s novim klijentom za sinkronizaciju servisa OneDrive](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) koji sadrži [datoteke na zahtjev](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="3057f-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="3057f-109">Pristupite svim datotekama na servisu OneDrive bez korištenja lokalnog prostora za pohranu.</span><span class="sxs-lookup"><span data-stu-id="3057f-109">Access all your files in OneDrive without using local storage space.</span></span>
  