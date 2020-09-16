---
title: Dozvole za kalendar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748785"
---
# <a name="calendar-permissions"></a><span data-ttu-id="c7433-102">Dozvole za kalendar</span><span class="sxs-lookup"><span data-stu-id="c7433-102">Calendar Permissions</span></span>

<span data-ttu-id="c7433-103">Korisnici mogu promijeniti vlastite dozvole za kalendar s programom Outlook na webu ili drugim klijentima, no kao administrator možda ćete morati istražiti i to.</span><span class="sxs-lookup"><span data-stu-id="c7433-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="c7433-104">Uz cmdlet sustava Exchange PowerShell prikazat će vam se dozvola na korisničkom kalendaru:</span><span class="sxs-lookup"><span data-stu-id="c7433-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="c7433-105">Dodatne informacije potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="c7433-105">To see more information see the following:</span></span>

- [<span data-ttu-id="c7433-106">Nabavite-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="c7433-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="c7433-107">Postavljanje-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="c7433-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="c7433-108">Dodavanje – MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="c7433-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="c7433-109">Dozvole za kalendar koriste se za zajedničko korištenje kalendara da biste vidjeli dodatne informacije o dijeljenjem kalendara programa Outlook, pogledajte ove članke:</span><span class="sxs-lookup"><span data-stu-id="c7433-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="c7433-110">Zajedničko korištenje kalendara programa Outlook s drugim osobama</span><span class="sxs-lookup"><span data-stu-id="c7433-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="c7433-111">Zajedničko korištenje kalendara u programu Outlook na webu za tvrtke</span><span class="sxs-lookup"><span data-stu-id="c7433-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="c7433-112">Da biste otklonili poteškoće s dozvolom kalendara, možete koristiti alat [Pomoćnik za podršku i oporavak](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="c7433-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>