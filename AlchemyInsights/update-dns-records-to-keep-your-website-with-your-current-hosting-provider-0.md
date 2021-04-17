---
title: Ažuriranje DNS zapisa da biste web-mjesto održavali kod trenutnog davatelja usluge hostiranja
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827502"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="b3d60-102">Ažuriranje DNS zapisa da biste web-mjesto održavali kod trenutnog davatelja usluge hostiranja</span><span class="sxs-lookup"><span data-stu-id="b3d60-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="b3d60-103">U centru za administratore sustava Microsoft 365 idite na stranicu Postavljanje domena, a zatim na popisu domena odaberite  >  [](https://admin.microsoft.com/Adminportal#/Domains) domenu koju koristite za web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="b3d60-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="b3d60-104">Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="b3d60-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="b3d60-105">Za **unos vrste DNS:A** **(Adresa)**</span><span class="sxs-lookup"><span data-stu-id="b3d60-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="b3d60-106">U **naziv glavnog računala ili Pseudonim** upišite sljedeće: **@**</span><span class="sxs-lookup"><span data-stu-id="b3d60-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="b3d60-107">Za **IP adresu** upišite statičnu IP adresu za web-mjesto na kojem se trenutno hostira (npr. 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="b3d60-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="b3d60-108">To mora biti  *statična*  IP adresa za web-mjesto, a ne  *dinamička*  IP adresa.</span><span class="sxs-lookup"><span data-stu-id="b3d60-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="b3d60-109">Provjerite s web-mjestom na kojem se hostira vaše web-mjesto da biste bili sigurni da možete dobiti statičnu IP adresu za javno web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="b3d60-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="b3d60-110">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="b3d60-110">Select **Save**.</span></span>

<span data-ttu-id="b3d60-111">Osim toga, možete stvoriti CNAME zapis da biste korisnicima pomogli pronaći vaše web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="b3d60-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="b3d60-112">Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="b3d60-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="b3d60-113">Za **vrstu DNS-a** unesite: **CNAME (pseudonim)**</span><span class="sxs-lookup"><span data-stu-id="b3d60-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="b3d60-114">Za **naziv glavnog računala ili Pseudonim** upišite sljedeće: **www**</span><span class="sxs-lookup"><span data-stu-id="b3d60-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="b3d60-115">U **okvir Upućuje na adresu** upišite potpuno kvalificirani naziv domene (FQDN) za web-mjesto (npr. contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b3d60-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="b3d60-116">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="b3d60-116">Select **Save**.</span></span>
