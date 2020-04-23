---
title: E-pošta tijeka rada nije poslana
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766125"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="2aaf3-102">E-pošta tijeka rada ne šalje se na popis ili biblioteku sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="2aaf3-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="2aaf3-103">E-pošta iz tijekova rada ne šalje se svim korisnicima ili samo određenim korisnicima ili vidite pogrešku **Poruka e-pošte ne može se poslati. Provjerite ima li e-pošta valjanog primatelja**.</span><span class="sxs-lookup"><span data-stu-id="2aaf3-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="2aaf3-104">Provjerite postoji li korisnik u grupi **Dozvole za sve osobe** (popis korisničkih informacija) za tu zbirku web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="2aaf3-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="2aaf3-105">Uzorak izravnog URL-a: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0</span><span class="sxs-lookup"><span data-stu-id="2aaf3-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="2aaf3-106">Ako korisnik ne postoji, provjerite je li korisnik prijavljen na stranicu.</span><span class="sxs-lookup"><span data-stu-id="2aaf3-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="2aaf3-107">Ako je to vanjski korisnik, provjerite je li prihvaćena njihova pozivnica.</span><span class="sxs-lookup"><span data-stu-id="2aaf3-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="2aaf3-108">Ako korisnik postoji u grupi dozvola, provjerite je li adresa e-pošte ispravna.</span><span class="sxs-lookup"><span data-stu-id="2aaf3-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="2aaf3-109">Ako adresa e-pošte korisnika nije postavljena ovdje, stvorite ogledno upozorenje za tog korisnika koje prisiljava sinkronizaciju tog korisničkog računa iz korisničkih profila sustava SharePoint s ovom zbirkom web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="2aaf3-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="2aaf3-110">E-pošta iz tijekova rada šalje se administratorima zbirke web-mjesta, ali ne i drugim korisnicima i vidjeti **pogrešku HTTP Zabranjeno <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="2aaf3-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="2aaf3-111">Pogledajte [Pristup odbijen prilikom slanja e-pošte sharepoint grupi](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="2aaf3-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="2aaf3-112">Provjerite i nije li aktivna značajka prikupljanja dozvola **za zaključavanje korisničkih dozvola s ograničenim pristupom.**</span><span class="sxs-lookup"><span data-stu-id="2aaf3-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="2aaf3-113">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="2aaf3-113">Related topics</span></span>
<span data-ttu-id="2aaf3-114">Želite li isprobati Microsoft Flow u sustavu SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="2aaf3-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="2aaf3-115">Stvori tijek</span><span class="sxs-lookup"><span data-stu-id="2aaf3-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="2aaf3-116">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="2aaf3-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


