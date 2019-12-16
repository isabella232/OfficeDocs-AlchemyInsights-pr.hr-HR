---
title: Samo za čitanje za poruku održavanja prilikom pokušaja korištenja sustava SharePoint ili servisa OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051273"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="01e77-102">Samo za čitanje za poruku održavanja prilikom pokušaja korištenja sustava SharePoint ili servisa OneDrive</span><span class="sxs-lookup"><span data-stu-id="01e77-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="01e77-103">Korisnici mogu primiti poruku **samo za čitanje za održavanje** kada pokušate koristiti SharePoint ili OneDrive za jedan od sljedećih scenarija.</span><span class="sxs-lookup"><span data-stu-id="01e77-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="01e77-104">Planirana ili aktivna aktivnost održavanja.</span><span class="sxs-lookup"><span data-stu-id="01e77-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="01e77-105">Provjerite ih navigacijom do centra za [poruke](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="01e77-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="01e77-106">Incident s visokim prioritetom, aktivni servis koji se možda javlja.</span><span class="sxs-lookup"><span data-stu-id="01e77-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="01e77-107">Provjerite ima li bilo kakvih savjetovanja/incidenata navigiranjem do [servisa Health](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="01e77-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="01e77-108">Manji scenarij oporavka iz automatskog ozdravljenja koji bi se mogao događati zbog neočekivanih događaja na poslužiteljima koji bi mogli trajati manje od 30 min.</span><span class="sxs-lookup"><span data-stu-id="01e77-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="01e77-109">Nema centra za poruke ni radnih mjesta za ova manja oporavka, ali biste se uskoro trebali vratiti u normalu.</span><span class="sxs-lookup"><span data-stu-id="01e77-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="01e77-110">U vrlo nekoliko navrata smo primijetili da je jedan od tri navedena scenarija bio uzrok, a servis je vraćen, ali korisnici cache preglednik nije očišćen.</span><span class="sxs-lookup"><span data-stu-id="01e77-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="01e77-111">Pokušajte izbrisati predmemoriju preglednika prije navigacije do web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="01e77-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="01e77-112">U pregledniku Microsoft Edge odaberite **Postavke**, a zatim odaberite **privatnost i sigurnost**.</span><span class="sxs-lookup"><span data-stu-id="01e77-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="01e77-113">Pod **jasnim pregledavanjem**odaberite **Odaberite što želite očistiti**.</span><span class="sxs-lookup"><span data-stu-id="01e77-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="01e77-114">Odaberite **Kolačići i spremljeni podaci web-mjesta**i odaberite **Očisti**.</span><span class="sxs-lookup"><span data-stu-id="01e77-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="01e77-115">Ovi koraci mogu se razlikovati prilikom korištenja drugih preglednika kao što su Mozilla Firefox ili Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="01e77-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="01e77-116">Druga bi mogućnost bila otvaranje SharePoint web-mjesta ili servisa OneDrive u novom prozoru InPrivate.</span><span class="sxs-lookup"><span data-stu-id="01e77-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>