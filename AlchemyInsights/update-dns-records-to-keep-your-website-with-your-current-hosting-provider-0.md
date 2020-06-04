---
title: Ažuriranje DNS zapisa radi održavanja web-mjesta kod trenutnog davatelja usluge hostiranja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665752"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="ec734-102">Ažuriranje DNS zapisa radi održavanja web-mjesta kod trenutnog davatelja usluge hostiranja</span><span class="sxs-lookup"><span data-stu-id="ec734-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="ec734-103">U centru za administratore sustava Microsoft **Setup**365  >  [otvorite](https://portal.office.com/adminportal/home#/Domains) stranicu Postava domene, a zatim na popisu domena odaberite domenu koju koristite za svoje web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="ec734-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="ec734-104">Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="ec734-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="ec734-105">Za **unos DNS vrste:** **A (Adresa)**</span><span class="sxs-lookup"><span data-stu-id="ec734-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="ec734-106">Za **naziv glavnog računala ili pseudonim**upišite sljedeće:**@**</span><span class="sxs-lookup"><span data-stu-id="ec734-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="ec734-107">Za **IP adresu**upišite statičku IP adresu web-lokacije na kojoj se trenutno hostira (na primjer, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="ec734-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="ec734-108">To mora biti *statička* IP adresa za web-mjesto, a ne *dinamička* IP adresa.</span><span class="sxs-lookup"><span data-stu-id="ec734-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="ec734-109">Provjerite s web-lokacijom na kojoj se nalazi vaše web-mjesto da biste bili sigurni da možete dobiti statičku IP adresu za javno web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="ec734-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="ec734-110">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="ec734-110">Select **Save**.</span></span>

<span data-ttu-id="ec734-111">Osim toga, možete stvoriti CNAME zapis da biste korisnicima pomogli pronaći vaše web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="ec734-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="ec734-112">Odaberite **+ Novi prilagođeni zapis** i unesite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="ec734-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="ec734-113">Za **DNS tip** ulaziti: **CNAME (Pseudonim)**</span><span class="sxs-lookup"><span data-stu-id="ec734-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="ec734-114">Za **naziv glavnog računala ili pseudonim**upišite sljedeće: **www**</span><span class="sxs-lookup"><span data-stu-id="ec734-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="ec734-115">Za **adrese upućuje na adresu**upišite potpuno kvalificirani naziv domene (FQDN) za web-mjesto (na primjer, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="ec734-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="ec734-116">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="ec734-116">Select **Save**.</span></span>
