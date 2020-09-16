---
title: Grupa šalji kao Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740143"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="3319a-102">Grupa šalji kao Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3319a-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="3319a-103">Možete dodijeliti dozvole Pošalji kao da biste određenim korisnicima dopustili da šalju poruke kao grupu Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="3319a-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="3319a-104">Spojite se na PowerShell sustava Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="3319a-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="3319a-105">Izvršite sljedeću naredbu:</span><span class="sxs-lookup"><span data-stu-id="3319a-105">Run the following command:</span></span>  

    <span data-ttu-id="3319a-106">Dodavanje-RecipientPermission `<GroupName>` -trustee `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="3319a-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="3319a-107">Dodatne informacije potražite u članku [Dopusti članovima da pošalju kao ili pošalju u ime grupe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="3319a-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>