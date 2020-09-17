---
title: Ažuriranje DNS zapisa radi zadržavanja web-mjesta s trenutnim davatelja usluga hostiranja
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815777"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="78fcb-102">Ažuriranje DNS zapisa radi zadržavanja web-mjesta s trenutnim davatelja usluga hostiranja</span><span class="sxs-lookup"><span data-stu-id="78fcb-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="78fcb-103">U centru za administratore sustava Microsoft 365 otvorite stranicu **Postavke**  >  [domene](https://admin.microsoft.com/Adminportal#/Domains) , a zatim na popisu domena odaberite domenu koju koristite za web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="78fcb-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="78fcb-104">Odaberite **+ novi prilagođeni zapis** pa unesite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="78fcb-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="78fcb-105">Za **vrstu DNS** -A unesite: **A (adresa)**</span><span class="sxs-lookup"><span data-stu-id="78fcb-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="78fcb-106">Za **naziv glavnog računala ili pseudonim**upišite sljedeće: **@**</span><span class="sxs-lookup"><span data-stu-id="78fcb-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="78fcb-107">Za **IP adresu**upišite STATIČNU IP adresu web-mjesta na kojoj je trenutno domaćin (na primjer,: 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="78fcb-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="78fcb-108">Ovo mora biti  *statična*  IP adresa za web-mjesto, a ne  *dinamička*  IP adresa.</span><span class="sxs-lookup"><span data-stu-id="78fcb-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="78fcb-109">Provjerite uz web-mjesto na kojem je web-mjesto hostirano da biste mogli nabaviti statičnu IP adresu za javno web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="78fcb-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="78fcb-110">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="78fcb-110">Select **Save**.</span></span>

<span data-ttu-id="78fcb-111">Osim toga, možete stvoriti CNAME zapis koji korisnicima olakšava pronalaženje web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="78fcb-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="78fcb-112">Odaberite **+ novi prilagođeni zapis** pa unesite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="78fcb-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="78fcb-113">Za **vrstu DNS** -a unesite: **CNAME (pseudonim)**</span><span class="sxs-lookup"><span data-stu-id="78fcb-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="78fcb-114">Za **naziv glavnog računala ili pseudonim**upišite sljedeće: **www**</span><span class="sxs-lookup"><span data-stu-id="78fcb-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="78fcb-115">Da **biste unijeli točku na adresu**, upišite potpuno kvalificirani naziv domene (FQDN) za vaše web-mjesto (primjerice, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="78fcb-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="78fcb-116">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="78fcb-116">Select **Save**.</span></span>
