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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655274"
---
# <a name="data-location"></a><span data-ttu-id="34832-102">Lokacija podataka</span><span class="sxs-lookup"><span data-stu-id="34832-102">Data location</span></span>

<span data-ttu-id="34832-103">Lokaciju klijenta možete vidjeti u centru za administratore ili povezivanjem sa sustavom Exchange Online putem komponente PowerShell.</span><span class="sxs-lookup"><span data-stu-id="34832-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="34832-104">**Centar za administratore:**</span><span class="sxs-lookup"><span data-stu-id="34832-104">**Admin center:**</span></span>
1. <span data-ttu-id="34832-105">Prijavite se u centar za [administratore](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="34832-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="34832-106">Odaberite**Profil organizacije** **postavki** > .</span><span class="sxs-lookup"><span data-stu-id="34832-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="34832-107">U **odjeljku Lokacija podataka**odaberite **Prikaz pojedinosti**.</span><span class="sxs-lookup"><span data-stu-id="34832-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="34832-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="34832-108">**PowerShell:**</span></span>
1. <span data-ttu-id="34832-109">Povežite se sa sustavom Exchange Online pomoću komponente Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="34832-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="34832-110">Izvršite cmdlet [Get-OrganizationUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) da biste prikazali popis svojstava klijenta.</span><span class="sxs-lookup"><span data-stu-id="34832-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="34832-111">Pogledaj vlasništvo OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="34832-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="34832-112">Kada imate lokaciju podataka za EXO i SPO, možete odrediti lokaciju podataka za druge usluge koje možete koristiti iz [mjesta gdje se nalaze vaši podaci](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="34832-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>