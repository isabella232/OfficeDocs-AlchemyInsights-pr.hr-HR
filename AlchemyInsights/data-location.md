---
title: Lokacija podataka
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627838"
---
# <a name="data-location"></a><span data-ttu-id="5782e-102">Lokacija podataka</span><span class="sxs-lookup"><span data-stu-id="5782e-102">Data location</span></span>

<span data-ttu-id="5782e-103">Mjesto vašeg Office 365 klijenta možete vidjeti u centru za administraciju ili povezivanjem s Exchange Online putem PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5782e-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="5782e-104">**Centar za administraciju:**</span><span class="sxs-lookup"><span data-stu-id="5782e-104">**Admin center:**</span></span>
1. <span data-ttu-id="5782e-105">Prijavite se u [centar za administraciju](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="5782e-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="5782e-106">Odaberite **Postavke** > **organizacije profil**.</span><span class="sxs-lookup"><span data-stu-id="5782e-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="5782e-107">U odjeljku **lokacija podataka**odaberite **Prikaz detalja**.</span><span class="sxs-lookup"><span data-stu-id="5782e-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="5782e-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="5782e-108">**PowerShell:**</span></span>
1. <span data-ttu-id="5782e-109">Povežite se s Exchangeovim internetom pomoću Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5782e-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="5782e-110">Izvršite cmdlet [Get-Organizatacionalunit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) da biste prikazali popis svojstava vašeg stanara.</span><span class="sxs-lookup"><span data-stu-id="5782e-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="5782e-111">Pogledajte svojstvo OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="5782e-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="5782e-112">Kada imate mjesto podataka za EXO i SPO, možete odrediti mjesto podataka za druge usluge koje možete koristiti na [mjestu gdje se nalaze vaši podaci](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="5782e-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>