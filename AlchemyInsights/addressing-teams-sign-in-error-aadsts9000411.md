---
title: Rješavanje problema s prijavom u timove za AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687030"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="c063c-102">Rješavanje problema s prijavom u timove za AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="c063c-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="c063c-103">Kada se prijavite u Microsoftove timove, možda će vam se prikazati pogreška: Žao nam je **, ali imamo problema s prijavom u AADSTS9000411: zahtjev nije pravilno oblikovan. Parametar "login_hint" dupliciran je.**</span><span class="sxs-lookup"><span data-stu-id="c063c-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="c063c-104">Da biste riješili taj problem, provjerite ažuriraju li se klijenti Microsoftova timova.</span><span class="sxs-lookup"><span data-stu-id="c063c-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="c063c-105">Dodatne informacije o ažuriranju klijenta potražite u članku [Ažuriranje Microsoftovih timova](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="c063c-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="c063c-106">Ako ne možete ažurirati klijenta iz nekog razloga, odprijavite se od klijenta koji će izbrisati većinu predmemoriranih podataka.</span><span class="sxs-lookup"><span data-stu-id="c063c-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="c063c-107">No ako i dalje imate problema nakon odjave/prijave, napustite timove i poništite svoj klijent predmemorija na sljedeći način:</span><span class="sxs-lookup"><span data-stu-id="c063c-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="c063c-108">Zatvaranje Microsoftovih timova.</span><span class="sxs-lookup"><span data-stu-id="c063c-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="c063c-109">Idite na:%AppData%\microsoft\timovi i izbrišite sve datoteke.</span><span class="sxs-lookup"><span data-stu-id="c063c-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="c063c-110">Ponovno otvorite Microsoftove timove.</span><span class="sxs-lookup"><span data-stu-id="c063c-110">Reopen Microsoft Teams.</span></span>
