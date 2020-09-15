---
title: Poruka o održavanju samo za čitanje prilikom pokušaja korištenja sustava SharePoint ili servisa OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670824"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="164b3-102">Poruka o održavanju samo za čitanje prilikom pokušaja korištenja sustava SharePoint ili servisa OneDrive</span><span class="sxs-lookup"><span data-stu-id="164b3-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="164b3-103">Prilikom pokušaja korištenja sustava SharePoint ili servisa OneDrive za jedan od sljedećih scenarija korisnici mogu primiti poruku **samo za čitanje** .</span><span class="sxs-lookup"><span data-stu-id="164b3-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="164b3-104">Planirana ili aktivna aktivnost održavanja.</span><span class="sxs-lookup"><span data-stu-id="164b3-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="164b3-105">Potražite ih tako da otvorite centar za [poruke](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="164b3-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="164b3-106">Problem s velikim prioritetom, aktivnim incidentom servisa koji se možda pojavljuje.</span><span class="sxs-lookup"><span data-stu-id="164b3-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="164b3-107">Provjerite postoje li Savjeti/incidenti tako da odete na [zdravlje servisa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="164b3-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="164b3-108">Manji scenario za automatsko ozdravljenje koji bi se mogao događati zbog neočekivanih događaja na poslužiteljima koji bi mogli trajati manje od 30 min ili više.</span><span class="sxs-lookup"><span data-stu-id="164b3-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="164b3-109">Nema centra za poruke ili zdravstvenih pošta za ove male oporavnice, no uskoro ćete se vratiti u normalu.</span><span class="sxs-lookup"><span data-stu-id="164b3-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="164b3-110">U vrlo malo navrata primijetili smo da je jedan od navedenih triju scenarija uzrok, a servis je vraćen, ali predmemorija korisnika preglednika nije očišćena.</span><span class="sxs-lookup"><span data-stu-id="164b3-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="164b3-111">Pokušajte izbrisati predmemoriranje preglednika prije nego što odete na web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="164b3-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="164b3-112">U pregledniku Microsoft Edge odaberite **Postavke**, a zatim odaberite **privatnost i sigurnost**.</span><span class="sxs-lookup"><span data-stu-id="164b3-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="164b3-113">U odjeljku **čisto pregledavanje**odaberite **Odaberi što želite očistiti**.</span><span class="sxs-lookup"><span data-stu-id="164b3-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="164b3-114">Odaberite **Kolačići i spremite podatke o web-mjestu**, a zatim odaberite **Očisti**.</span><span class="sxs-lookup"><span data-stu-id="164b3-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="164b3-115">Ovi se koraci mogu razlikovati prilikom korištenja drugih preglednika, kao što su Mozilla Firefox ili Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="164b3-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="164b3-116">Druga bi mogućnost bila otvaranje web-mjesta sustava SharePoint ili servisa OneDrive u novom prozoru weba InPrivate.</span><span class="sxs-lookup"><span data-stu-id="164b3-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>