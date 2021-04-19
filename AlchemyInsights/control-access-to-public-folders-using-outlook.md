---
title: Upravljanje pristupom javnim mapama pomoću programa Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816732"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="894d7-102">Upravljanje pristupom javnim mapama pomoću programa Outlook</span><span class="sxs-lookup"><span data-stu-id="894d7-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="894d7-103">Da biste upravljali korisnicima koji mogu pristupati javnim mapama pomoću programa Outlook:</span><span class="sxs-lookup"><span data-stu-id="894d7-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="894d7-104">Korištenje `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="894d7-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="894d7-105">$true: omogući korisnicima pristup javnim mapama u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="894d7-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="894d7-106">$false: onemogućivanje korisničkog pristupa javnim mapama u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="894d7-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="894d7-107">To je zadana vrijednost.</span><span class="sxs-lookup"><span data-stu-id="894d7-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="894d7-108">Napomena: ovim postupkom možete upravljati samo vezama s klijentima programa Outlook za računala za Windows.</span><span class="sxs-lookup"><span data-stu-id="894d7-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="894d7-109">Korisnici mogu nastaviti pristupati javnim mapama pomoću aplikacije OWA ili Outlook za Mac.</span><span class="sxs-lookup"><span data-stu-id="894d7-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="894d7-110">Dodatne informacije potražite u članku [Kontrolirane veze s javnim mapama u programu Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="894d7-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
