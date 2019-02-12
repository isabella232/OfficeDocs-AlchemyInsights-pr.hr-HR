---
title: Ažuriranje zapisa DNS zadržati svoje web-mjesto s trenutnom pružatelju usluge
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: e0dadba1e3ffd1cf0d49c0a76ec2efbbc6ae92db
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906112"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="d44a2-102">Ažuriranje zapisa DNS zadržati svoje web-mjesto s trenutnom pružatelju usluge</span><span class="sxs-lookup"><span data-stu-id="d44a2-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="d44a2-103">Na stranici [domena](https://portal.office.com/adminportal/home#/Domains) popisa domena, odaberite domene koristite za vaše web-mjesto, a zatim odaberite **postavke DNS** u okno upravljanje.</span><span class="sxs-lookup"><span data-stu-id="d44a2-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="d44a2-104">Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="d44a2-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="d44a2-105">**Vrsta DNS** unesite: **(adresa)**</span><span class="sxs-lookup"><span data-stu-id="d44a2-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="d44a2-106">Za **naziv glavnog računala ili pseudonim**, upišite sljedeće:**@**</span><span class="sxs-lookup"><span data-stu-id="d44a2-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="d44a2-107">Za **IP adresu**, upišite statičku IP adresu za vaše web-mjesto gdje ga trenutno hostuje (na primjer, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="d44a2-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="d44a2-p101">To mora biti *statička* IP adresa za web-mjesto, ne *dinamičku* IP adresu. Provjerite s gdje je smještena vaše web-mjesto za dobivanje statičku IP adresu za vaše javne web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="d44a2-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="d44a2-110">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="d44a2-110">Select **Save**.</span></span> 
    
<span data-ttu-id="d44a2-111">Osim toga, možete stvoriti zapis CNAME pomoći klijentima da pronađu vaše web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="d44a2-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="d44a2-112">Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="d44a2-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="d44a2-113">**Vrsta DNS** unesite: **CNAME (pseudonima)**</span><span class="sxs-lookup"><span data-stu-id="d44a2-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="d44a2-114">Za **naziv glavnog računala ili pseudonim**, upišite sljedeće: **www**</span><span class="sxs-lookup"><span data-stu-id="d44a2-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="d44a2-115">**Točke adresu**, upišite je potpuno kvalificirani naziv domene (FQDN) za web-mjesto (na primjer, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="d44a2-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="d44a2-116">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="d44a2-116">Select **Save**.</span></span> 
    

