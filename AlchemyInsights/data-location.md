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
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207253"
---
# <a name="data-location"></a><span data-ttu-id="3feb8-102">Lokacija podataka</span><span class="sxs-lookup"><span data-stu-id="3feb8-102">Data location</span></span>

<span data-ttu-id="3feb8-103">Mjesto vašeg Office 365 klijenta možete vidjeti u centru za administraciju ili povezivanjem s Exchange Online putem PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3feb8-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="3feb8-104">**Centar za administraciju:**</span><span class="sxs-lookup"><span data-stu-id="3feb8-104">**Admin center:**</span></span>
1. <span data-ttu-id="3feb8-105">Prijavite se u [centar za administraciju](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="3feb8-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="3feb8-106">Odaberite **Postavke** > **organizacije profil**.</span><span class="sxs-lookup"><span data-stu-id="3feb8-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="3feb8-107">U odjeljku **lokacija podataka**odaberite **Prikaz detalja**.</span><span class="sxs-lookup"><span data-stu-id="3feb8-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="3feb8-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="3feb8-108">**PowerShell:**</span></span>
1. <span data-ttu-id="3feb8-109">Povežite se s Exchangeovim internetom pomoću Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3feb8-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="3feb8-110">Izvršite cmdlet [Get-Organizatacionalunit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) da biste prikazali popis svojstava vašeg stanara.</span><span class="sxs-lookup"><span data-stu-id="3feb8-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="3feb8-111">Pogledajte svojstvo OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="3feb8-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="3feb8-112">Kada imate mjesto podataka za EXO i SPO, možete odrediti mjesto podataka za druge usluge koje možete koristiti na [mjestu gdje se nalaze vaši podaci](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="3feb8-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>