---
title: Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523382"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="acc81-102">Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi</span><span class="sxs-lookup"><span data-stu-id="acc81-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="acc81-103">Slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="acc81-103">Follow these steps:</span></span>

1. <span data-ttu-id="acc81-104">Ako niste globalni administrator, da biste potražili poruke, vaš račun mora biti dodan u **grupu uloga menadžera za istraživanje** ili za **Upravljanje usklađivanjem pretraživanja**.</span><span class="sxs-lookup"><span data-stu-id="acc81-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="acc81-105">Da biste izbrisali poruke, morat ćete se pridružiti **grupi uloga za upravljanje organizacijom** ili **ulogu pretraživanja i brisanja**.</span><span class="sxs-lookup"><span data-stu-id="acc81-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="acc81-106">Dozvole za te uloge dodijeljene su u [centru za sigurnost & usklađenosti.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="acc81-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="acc81-107">[Stvorite pretraživanje sadržaja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku koja će se izbrisati.</span><span class="sxs-lookup"><span data-stu-id="acc81-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="acc81-108">[Spojite se na sigurnosnu & PowerShell centra za usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="acc81-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="acc81-109">Ako koristite MFA, pogledajte ove upute: [Povezivanje s pomoću komponente Security & u centru za usklađenost s višestrukim čimbenikom provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="acc81-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="acc81-110">Izbrišite poruku: Pokrenite `New-ComplianceSearchAction` cmdlet da biste izbrisali poruku.</span><span class="sxs-lookup"><span data-stu-id="acc81-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="acc81-111">Izbrisane poruke premještaju se u korisničku mapu stavke koje se mogu oporaviti.</span><span class="sxs-lookup"><span data-stu-id="acc81-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="acc81-112">Naredba primjer potražite u odjeljku [treći korak: brisanje poruke.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="acc81-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
