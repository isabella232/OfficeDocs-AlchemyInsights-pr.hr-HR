---
title: E-pošta tijeka rada se ne šalje
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049365"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="e126c-102">E-pošta tijeka rada ne šalje se za SharePointov popis ili biblioteku</span><span class="sxs-lookup"><span data-stu-id="e126c-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="e126c-103">E-pošta iz tijekova rada ne šalju se svim korisnicima ili samo određenim korisnicima ili vidite pogrešku **koju poruka e-pošte ne može poslati. Provjerite ima li e-pošta valjanog primatelja**.</span><span class="sxs-lookup"><span data-stu-id="e126c-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="e126c-104">Provjerite postoji li korisnik u grupi dozvola za **sve osobe** (popis korisničkih informacija) za tu zbirku web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="e126c-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="e126c-105">Primjer Direct URL: https://<tenant>. sharepoint.com/sites/<sitename>/_layouts/15/. aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="e126c-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="e126c-106">Ako korisnik ne postoji, provjerite je li korisnik potpisan na stranicu.</span><span class="sxs-lookup"><span data-stu-id="e126c-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="e126c-107">Ako je to vanjski korisnik, provjerite je li njihova pozivnica prihvaćena.</span><span class="sxs-lookup"><span data-stu-id="e126c-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="e126c-108">Ako korisnik postoji u grupi dozvola, provjerite je li adresa e-pošte točna.</span><span class="sxs-lookup"><span data-stu-id="e126c-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="e126c-109">Ako adresa e-pošte korisnika nije postavljena ovdje, zatim stvorite upozorenje uzorka za tog korisnika koji tjera sinkronizaciju tog korisničkog računa iz korisničkih profila sustava SharePoint u ovu zbirku web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="e126c-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="e126c-110">E-pošta iz tijekova rada šalju se administratorima zbirke web-mjesta, ali ne i drugim korisnicima i vidjeti pogrešku **http zabranjeno <span>https:</span>, url/_vti_bin/Client.XVC.SP.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="e126c-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="e126c-111">Pogledajte [pristup odbijen prilikom slanja e-pošte u SharePoint grupu](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="e126c-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="e126c-112">Također provjerite nije li aktivna značajka prikupljanja **dopuštenja za korisnike ograničenog pristupa** .</span><span class="sxs-lookup"><span data-stu-id="e126c-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="e126c-113">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="e126c-113">Related topics</span></span>
<span data-ttu-id="e126c-114">Želite li isprobati Microsoft Flow u sustavu SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="e126c-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="e126c-115">Stvori tok</span><span class="sxs-lookup"><span data-stu-id="e126c-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e126c-116">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="e126c-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


