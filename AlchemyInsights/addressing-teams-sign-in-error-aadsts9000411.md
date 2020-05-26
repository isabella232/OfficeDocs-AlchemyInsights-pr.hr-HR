---
title: Rješavanje pogreške prilikom prijave timova AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357400"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="aaf4b-102">Rješavanje pogreške prilikom prijave timova AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="aaf4b-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="aaf4b-103">Prilikom prijave u Microsoft Teams možda ćete primiti pogrešku: **Nažalost, ali imamo poteškoća s potpisivanjem u aADSTS9000411: zahtjev nije ispravno formatiran. Parametar "login_hint" je dupliciran.**</span><span class="sxs-lookup"><span data-stu-id="aaf4b-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="aaf4b-104">Da biste riješili taj problem, provjerite jesu li vaši klijenti sustava Microsoft Teams ažurirani.</span><span class="sxs-lookup"><span data-stu-id="aaf4b-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="aaf4b-105">Dodatne informacije o ažuriranju klijenta potražite u [odjeljku Ažuriranje servisa Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="aaf4b-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="aaf4b-106">Ako iz nekog razloga ne možete ažurirati klijenta, odjavom s klijenta izbrisat će se većina predmemorirane podatke.</span><span class="sxs-lookup"><span data-stu-id="aaf4b-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="aaf4b-107">Međutim, ako i dalje imate problema nakon odjave/prijave, zatvorite Teams i izbrišite predmemoriju klijenta na sljedeći način:</span><span class="sxs-lookup"><span data-stu-id="aaf4b-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="aaf4b-108">Zatvorite Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="aaf4b-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="aaf4b-109">Idite na: %appdata%\microsoft\teams i izbrišite sve datoteke.</span><span class="sxs-lookup"><span data-stu-id="aaf4b-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="aaf4b-110">Ponovno otvorite Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="aaf4b-110">Reopen Microsoft Teams.</span></span>
