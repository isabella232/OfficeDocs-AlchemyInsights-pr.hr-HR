---
title: Otklanjanje poteškoća s sinkronizacijom lozinke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664918"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="9ec3c-102">Otklanjanje poteškoća s sinkronizacijom lozinke</span><span class="sxs-lookup"><span data-stu-id="9ec3c-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="9ec3c-103">Da biste otklonili poteškoće s sinkronizacijom lozinki, započnite pomoću tog zadatka AAD Connect otklanjanje poteškoća da biste utvrdili zašto se lozinke ne sinkroniziraju.</span><span class="sxs-lookup"><span data-stu-id="9ec3c-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="9ec3c-104">Da biste započeli, otvorite [Upravljanje izravnim sinkronizacijom](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="9ec3c-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="9ec3c-105">Otvorite novu sesiju komponente Windows PowerShell na poslužitelju Azure AD Connect, a zatim odaberite mogućnost **Pokreni kao administrator** .</span><span class="sxs-lookup"><span data-stu-id="9ec3c-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="9ec3c-106">Pokretanje pravilnika za Remotepotpisana ili skupa izvršnih pravila za postavljanje pogubljenja</span><span class="sxs-lookup"><span data-stu-id="9ec3c-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="9ec3c-107">Pokrenite čarobnjak za Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9ec3c-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="9ec3c-108">Idite na stranicu dodatni zadaci > **Otklanjanje poteškoća**  >  **dalje**.</span><span class="sxs-lookup"><span data-stu-id="9ec3c-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="9ec3c-109">Odaberite **Pokreni** da biste otvorili izbornik otklanjanja poteškoća sa pomoću komponente PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9ec3c-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="9ec3c-110">Odaberite **Otklanjanje poteškoća s sinkronizacijom lozinke**.</span><span class="sxs-lookup"><span data-stu-id="9ec3c-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="9ec3c-111">Problem je obično što lozinka nije sinkronizirana za određeni korisnički račun.</span><span class="sxs-lookup"><span data-stu-id="9ec3c-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="9ec3c-112">**Bilješke** Sinkronizacija lozinke neće uspjeti ako je posljednja uspješna sinkronizacija lozinki bila prije nekog vremena.</span><span class="sxs-lookup"><span data-stu-id="9ec3c-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="9ec3c-113">Dodatne informacije o otklanjanju poteškoća s sinkronizacijom lozinke potražite [u članku Otklanjanje poteškoća s sinkronizacijom lozinke uz sinkronizaciju servisa Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="9ec3c-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>