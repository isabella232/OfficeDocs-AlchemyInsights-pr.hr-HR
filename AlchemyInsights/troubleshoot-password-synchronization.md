---
title: Rješavanje problema s lozinku sinkronizacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767168"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="e8bf2-102">Rješavanje problema s lozinku sinkronizacije</span><span class="sxs-lookup"><span data-stu-id="e8bf2-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="e8bf2-103">Otklanjanje poteškoća gdje nema lozinke su sinkronizirane s verzijom Azure AD povezivanje 1.1.614.0 ili noviji:</span><span class="sxs-lookup"><span data-stu-id="e8bf2-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="e8bf2-104">Otvorite novu sesiju Windows PowerShell na poslužitelju Azure AD povezivanje s mogućnost **Pokreni kao Administrator** .</span><span class="sxs-lookup"><span data-stu-id="e8bf2-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="e8bf2-105">Pokrenite **RemoteSigned skup pravilnik izvođenja** ili **Postavi pravilnik izvođenja neograničen**.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="e8bf2-106">Pokretanje čarobnjaka za povezivanje Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="e8bf2-107">Idite na \*\* dodatnih zadataka \*\* stranice, odaberite \*\* otklanjanje \*\*, i pritisnite **Dalje**.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="e8bf2-108">Na stranici otklanjanje poteškoća kliknite izbornik **pokretanje pokrenuti otklanjanje pogrešaka** u PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="e8bf2-109">U glavnom izborniku odaberite **Otklanjanje sinkronizacije lozinku**.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="e8bf2-110">U izborniku sub odaberite **lozinku sinkronizacije neće raditi uopće**.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="e8bf2-111">**Razumjeli rezultate otklanjanje zadatka**</span><span class="sxs-lookup"><span data-stu-id="e8bf2-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="e8bf2-112">Otklanjanje poteškoća zadatak izvodi sljedeće čekove:</span><span class="sxs-lookup"><span data-stu-id="e8bf2-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="e8bf2-113">Ovjerava za klijentske Azure AD omogućena značajka sinkronizacije lozinku.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="e8bf2-114">Ovjerava da poslužitelj Azure AD povezivanje nije u pripremne načinu.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="e8bf2-115">Za svaki postojeći lokalno Active Directory poveznik (koji odgovara postojećem šume servisa Active Directory):</span><span class="sxs-lookup"><span data-stu-id="e8bf2-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="e8bf2-116">Provjerava je li omogućena značajka sinkronizacije lozinku.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="e8bf2-117">Traži lozinku sinkronizacije pulsnom događaje u zapisnicima događaja aplikacija sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="e8bf2-118">Za svaku domenu Active Directory pod Active Directory poveznik lokalno:</span><span class="sxs-lookup"><span data-stu-id="e8bf2-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="e8bf2-119">Ovjerava domena je dostupno s poslužitelja Azure AD povezivanje.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="e8bf2-120">Ovjerava računi Active Directory Domain Services (AD DS) koje koriste Active Directory poveznik lokalno ima ispravan korisničko ime, lozinku i dozvole potrebne za sinkronizaciju lozinku.</span><span class="sxs-lookup"><span data-stu-id="e8bf2-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="e8bf2-121">Više pomoć sinkronizaciju lozinku za otklanjanje poteškoća potražite [Otklanjanje lozinku sinkronizacije s Azure AD povezivanje sinkronizaciju](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="e8bf2-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

