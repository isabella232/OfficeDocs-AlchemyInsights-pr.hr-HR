---
title: Brisanje privatnog kanala timova
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730907"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="002e8-102">Brisanje privatnog kanala timova</span><span class="sxs-lookup"><span data-stu-id="002e8-102">Delete a Teams private channel</span></span>

<span data-ttu-id="002e8-103">Microsoft je svjestan problema s brisanjem privatnog kanala timova ako su pravila zadržavanja sustava SharePoint omogućena za web-mjesto sustava SharePoint u podlozi.</span><span class="sxs-lookup"><span data-stu-id="002e8-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="002e8-104">Microsoft radi na ispravcima.</span><span class="sxs-lookup"><span data-stu-id="002e8-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="002e8-105">U međuvremenu možete izbrisati privatni kanal pomoću sljedećih zaobilaznih rješenja.</span><span class="sxs-lookup"><span data-stu-id="002e8-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="002e8-106">**Izuzimanje tima/zbirke web-mjesta iz pravilnika o zadržavanju sustava SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="002e8-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="002e8-107">Idite na portal za administratore sustava Office 365, a zatim odaberite **Prikaz svih** u lijevoj navigacijskom oknu.</span><span class="sxs-lookup"><span data-stu-id="002e8-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="002e8-108">U odjeljku **centri za administratore**idite na **Sigurnosno &**  >  pravilnik o**sprječavanju gubitka podataka**  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="002e8-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="002e8-109">Odredite pravila koja se odnose na web-mjesta sustava SharePoint i izmijenite pravilo tako da web-mjesto sustava SharePoint za tim koji sadrži privatni kanal nije obuhvaćeno Pravilnikom o zadržavanju.</span><span class="sxs-lookup"><span data-stu-id="002e8-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="002e8-110">Spremanje pravilnika.</span><span class="sxs-lookup"><span data-stu-id="002e8-110">Save the policy.</span></span>
    <span data-ttu-id="002e8-111">Postavke pravilnika mogu potrajati i do 24 sata.</span><span class="sxs-lookup"><span data-stu-id="002e8-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="002e8-112">Kada je web-mjesto isključeno, možete izbrisati privatni kanal.</span><span class="sxs-lookup"><span data-stu-id="002e8-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="002e8-113">***Možda*** ćete moći izbrisati privatni kanal pomoću Microsoftovih timova na uređaju sa sustavom Android.</span><span class="sxs-lookup"><span data-stu-id="002e8-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="002e8-114">Za srodne informacije sustava SharePoint pročitajte članak [nije moguće izbrisati stavke u sustavu SharePoint Online ni na servisu OneDrive za tvrtke](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="002e8-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>