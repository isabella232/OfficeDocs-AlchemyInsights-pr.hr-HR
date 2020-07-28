---
title: Brisanje privatnog kanala za timove
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438837"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="b8788-102">Brisanje privatnog kanala za timove</span><span class="sxs-lookup"><span data-stu-id="b8788-102">Delete a Teams private channel</span></span>

<span data-ttu-id="b8788-103">Microsoft je svjestan problema prilikom brisanja privatnog kanala teams ako su za temeljno web-mjesto sustava SharePoint omogućena pravila zadržavanja sustava SharePoint sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b8788-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="b8788-104">Microsoft radi na popravku.</span><span class="sxs-lookup"><span data-stu-id="b8788-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="b8788-105">U međuvremenu, možete koristiti sljedeća zaobilazna rješenja za brisanje privatnog kanala.</span><span class="sxs-lookup"><span data-stu-id="b8788-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="b8788-106">**Izuzmite zbirku tima/web-mjesta iz pravila zadržavanja sustava Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="b8788-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="b8788-107">Idite na portal za administratore sustava Office 365 i odaberite **Prikaži sve** u lijevom navigacijskom oknu.</span><span class="sxs-lookup"><span data-stu-id="b8788-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="b8788-108">U **odjeljku Centri za administratore**idite na Pravila o **Security & Compliance**  >  **sprječavanju gubitka podataka o**sigurnosti &  >  **Policy**usklađenosti .</span><span class="sxs-lookup"><span data-stu-id="b8788-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="b8788-109">Prepoznajte sva pravila koja se primjenjuju na web-mjesta sustava SharePoint i izmijenite pravila tako da Sharepoint web-mjesto tima koji sadrži privatni kanal nije uključeno u pravila zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="b8788-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="b8788-110">Spremite pravila.</span><span class="sxs-lookup"><span data-stu-id="b8788-110">Save the policy.</span></span>
    <span data-ttu-id="b8788-111">Postavke pravila mogu potrajati do 24 sata.</span><span class="sxs-lookup"><span data-stu-id="b8788-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="b8788-112">Nakon isključivanja web-mjesta možete izbrisati privatni kanal.</span><span class="sxs-lookup"><span data-stu-id="b8788-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="b8788-113">***Možda ćete*** moći izbrisati privatni kanal pomoću servisa Microsoft Teams na Android uređaju.</span><span class="sxs-lookup"><span data-stu-id="b8788-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="b8788-114">Povezane informacije sustava SharePoint [potražite u odjeljku Brisanje stavki u sustavima SharePoint Online ili OneDrive za tvrtke](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="b8788-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>