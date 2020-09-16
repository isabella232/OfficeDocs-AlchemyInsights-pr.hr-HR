---
title: E-pošta tijeka rada ne šalje se
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748981"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="5f275-102">E-pošta tijeka rada ne šalje se na popis ili biblioteku sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="5f275-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="5f275-103">E-pošta iz tijekova rada ne šalje se svim korisnicima ili samo određenim korisnicima ili vam se prikazuje pogreška **poruke e-pošte nije moguće poslati. Provjerite ima li e-pošta valjani primatelj**.</span><span class="sxs-lookup"><span data-stu-id="5f275-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="5f275-104">Provjerite postoji li korisnik u grupi dozvole za **sve osobe** (popis korisničkih informacija) za tu zbirku web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="5f275-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="5f275-105">Ogledni Direktni URL: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/People.aspx? Člana Članigrupe = 0</span><span class="sxs-lookup"><span data-stu-id="5f275-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="5f275-106">Ako korisnik ne postoji, provjerite je li korisnik potpisan na stranicu.</span><span class="sxs-lookup"><span data-stu-id="5f275-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="5f275-107">Ako se radi o vanjskom korisniku, provjerite je li pozivnica prihvaćena.</span><span class="sxs-lookup"><span data-stu-id="5f275-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="5f275-108">Ako korisnik postoji u grupi dozvole, provjerite je li adresa e-pošte točna.</span><span class="sxs-lookup"><span data-stu-id="5f275-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="5f275-109">Ako adresa e-pošte korisnika nije postavljena ovdje, stvorite ogledno upozorenje za tog korisnika koji prisiljava sinkronizaciju tog korisničkog računa iz korisničkih profila sustava SharePoint na ovu zbirku web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="5f275-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="5f275-110">E-pošta iz tijekova rada šalje se administratorima zbirke web-mjesta, ali ne i drugim korisnicima i prikazuje pogrešku **http zabranjen za <span>https:</span>/_vti_bin/Client.XVC.SP.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="5f275-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="5f275-111">Prikaz [odbijanja kada šaljete poruku e-pošte u grupu sustava SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="5f275-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="5f275-112">Provjerite i je li funkcija **ograničen pristup korisničkim dozvolama za zaključavanje** web-mjesta aktivna.</span><span class="sxs-lookup"><span data-stu-id="5f275-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="5f275-113">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="5f275-113">Related topics</span></span>
<span data-ttu-id="5f275-114">Želite li isprobati Microsoft Flow u sustavu SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="5f275-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="5f275-115">Stvaranje toka</span><span class="sxs-lookup"><span data-stu-id="5f275-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="5f275-116">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="5f275-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


