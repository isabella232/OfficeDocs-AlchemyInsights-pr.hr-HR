---
title: Rješavanje problema sa sinkronizacijom lozinkom
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387869"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="c15e7-102">Rješavanje problema sa sinkronizacijom lozinkom</span><span class="sxs-lookup"><span data-stu-id="c15e7-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="c15e7-103">Da biste otklonili poteškoće sa sinkronizacijom lozinkom, pokrenite ovaj zadatak za otklanjanje poteškoća s AAD Connectom da biste odredili zašto se lozinke ne sinkroniziraju.</span><span class="sxs-lookup"><span data-stu-id="c15e7-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="c15e7-104">Da biste započeli, idite na [Upravljanje izravnom sinkronizacijom](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="c15e7-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="c15e7-105">Otvorite novu sesiju komponente Windows PowerShell na poslužitelju Azure AD Connect i odaberite mogućnost **Pokreni kao administrator.**</span><span class="sxs-lookup"><span data-stu-id="c15e7-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="c15e7-106">Pokrenite Set-ExecutionPolicy RemoteSigned ili Set-ExecutionPolicy neograničeno.</span><span class="sxs-lookup"><span data-stu-id="c15e7-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="c15e7-107">Pokrenite čarobnjak za Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c15e7-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="c15e7-108">Idite na stranicu Dodatni zadaci > **Otklanjanje poteškoća**  >  **Sljedeće**.</span><span class="sxs-lookup"><span data-stu-id="c15e7-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="c15e7-109">Odaberite **Pokreni** da biste otvorili izbornik za otklanjanje poteškoća sa ljuskom PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c15e7-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="c15e7-110">Odaberite **Otklanjanje poteškoća sa sinkronizacijom lozinke**.</span><span class="sxs-lookup"><span data-stu-id="c15e7-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="c15e7-111">Problem je obično u tome što lozinka nije sinkronizirana za određeni korisnički račun.</span><span class="sxs-lookup"><span data-stu-id="c15e7-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="c15e7-112">**Bilješke** Sinkronizacija lozinkom ne uspijeva ako je posljednja uspješna sinkronizacija lozinke bila prije nekog vremena.</span><span class="sxs-lookup"><span data-stu-id="c15e7-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="c15e7-113">Dodatna pomoć za otklanjanje poteškoća sa sinkronizacijom [lozinkom potražite u članku Otklanjanje poteškoća sa sinkronizacijom raspršilim lozinkom sa sinkronizacijom azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="c15e7-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>