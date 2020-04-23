---
title: Rješavanje problema sa sinkronizacijom lozinki
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732502"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="e5a8f-102">Rješavanje problema sa sinkronizacijom lozinki</span><span class="sxs-lookup"><span data-stu-id="e5a8f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="e5a8f-103">Da biste otklonili poteškoće kada se lozinke ne sinkroniziraju sa servisom Azure AD Connect verzije 1.1.614.0 ili novije:</span><span class="sxs-lookup"><span data-stu-id="e5a8f-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="e5a8f-104">Otvorite novu sesiju komponente Windows PowerShell na poslužitelju Azure AD Connect pomoću mogućnosti **Pokreni kao administrator.**</span><span class="sxs-lookup"><span data-stu-id="e5a8f-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="e5a8f-105">Pokrenite **Set-ExecutionPolicy RemoteSigned** ili **Set-ExecutionPolicy neograničen**.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="e5a8f-106">Pokrenite čarobnjak za Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="e5a8f-107">Idite na stranicu **Dodatni zadaci,** odaberite **Otklanjanje poteškoća**i kliknite **Dalje**.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="e5a8f-108">Na stranici Otklanjanje poteškoća kliknite **Pokreni da biste pokrenuli** izbornik za otklanjanje poteškoća u programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="e5a8f-109">U glavnom izborniku odaberite **Otklanjanje poteškoća sa sinkronizacijom lozinki**.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="e5a8f-110">U podizborniku odaberite **Sinkronizacija lozinki uopće ne funkcionira**.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="e5a8f-111">**Objašnjenje rezultata zadatka otklanjanja poteškoća**</span><span class="sxs-lookup"><span data-stu-id="e5a8f-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="e5a8f-112">Zadatak otklanjanja poteškoća izvodi sljedeće provjere:</span><span class="sxs-lookup"><span data-stu-id="e5a8f-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="e5a8f-113">Provjerava je li značajka sinkronizacije lozinke omogućena za klijenta Azure AD-a.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="e5a8f-114">Provjerava je li poslužitelj Azure AD Connect u pripremnom načinu rada.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="e5a8f-115">Za svaki postojeći lokalni konektor servisa Active Directory (koji odgovara postojećoj šumi servisa Active Directory):</span><span class="sxs-lookup"><span data-stu-id="e5a8f-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="e5a8f-116">Provjerava je li omogućena značajka sinkronizacije lozinke.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="e5a8f-117">Traži događaje zapisnika zapisnika zapisnika sinkronizacije lozinkom u zapisnicima događaja aplikacije sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="e5a8f-118">Za svaku domenu servisa Active Directory pod lokalnim povezom servisa Active Directory:</span><span class="sxs-lookup"><span data-stu-id="e5a8f-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="e5a8f-119">Provjerava je li domena dostupna s poslužitelja Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="e5a8f-120">Provjerava ima li računi servisa Active Directory Domain Services (AD DS) koje koristi lokalni poveznik servisa Active Directory ispravno korisničko ime, lozinku i dozvole potrebne za sinkronizaciju lozinki.</span><span class="sxs-lookup"><span data-stu-id="e5a8f-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="e5a8f-121">Dodatne informacije o otklanjanju poteškoća pri sinkronizaciji lozinki [potražite u članku Otklanjanje poteškoća sa sinkronizacijom lozinke pomoću sinkronizacije usluge Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="e5a8f-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  