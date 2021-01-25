---
title: Arhivski poštanski sandučić gotovo je pun
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974211"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="24358-102">Arhivski poštanski sandučić gotovo je pun</span><span class="sxs-lookup"><span data-stu-id="24358-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="24358-103">Ako korisnik primi upozorenje, **Poštanski sandučić arhive gotovo je pun** ili morate povećati veličinu njihovog arhivskog poštanskog sandučića, evo nekoliko savjeta:</span><span class="sxs-lookup"><span data-stu-id="24358-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="24358-104">Ako je korisniku dodijeljen plan sustava Exchange Online 1, nadogradite ga na licencu za **Exchange Online tarifu 2** da biste povećali veličinu od 50 GB do 100gb.</span><span class="sxs-lookup"><span data-stu-id="24358-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="24358-105">Ako je korisniku već dodijeljen neki od sljedećih načina: **Exchange Online tarifa 2** ili tarifa za Exchange Online 1 s dodacima za arhiviranje sustava Exchange Online, upotrijebite upute u nastavku da biste omogućili automatsko proširenje arhiviranja:.</span><span class="sxs-lookup"><span data-stu-id="24358-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="24358-106">[Spojite se na PowerShell sustava Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="24358-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="24358-107">Pokrenite sljedeći cmdlet za korisnika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="24358-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="24358-108">Pokrenite sljedeći cmdlet da biste potvrdili da je omogućen za korisnika:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="24358-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="24358-109">Dodatne informacije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="24358-109">For more information see:</span></span>

- [<span data-ttu-id="24358-110"> Omogućivanje neograničenog arhiviranja-pomoć za administratore – Microsoft 365 sukladnost | Microsoftovi dokumenti</span><span class="sxs-lookup"><span data-stu-id="24358-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="24358-111">Ograničenja sustava Exchange Online – opisi servisa | Microsoftovi dokumenti</span><span class="sxs-lookup"><span data-stu-id="24358-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="24358-112">Nadogradnja na neki drugi poslovni plan | Microsoftovi dokumenti</span><span class="sxs-lookup"><span data-stu-id="24358-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

