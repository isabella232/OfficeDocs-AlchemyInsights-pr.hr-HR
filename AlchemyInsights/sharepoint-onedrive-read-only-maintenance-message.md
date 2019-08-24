---
title: Za održavanje poruku kada pokušavate koristiti SharePoint ili OneDrive samo za čitanje
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620715"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="52a6e-102">Za održavanje poruku kada pokušavate koristiti SharePoint ili OneDrive samo za čitanje</span><span class="sxs-lookup"><span data-stu-id="52a6e-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="52a6e-103">Korisnici mogu primati poruke **Samo za čitanje za održavanje** kada pokušavate koristiti SharePoint ili OneDrive za jednu od sljedeće scenarije.</span><span class="sxs-lookup"><span data-stu-id="52a6e-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="52a6e-104">Planirani ili aktivni održavanja aktivnosti.</span><span class="sxs-lookup"><span data-stu-id="52a6e-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="52a6e-105">Provjerite ih odlaskom na [Poruku centar](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="52a6e-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="52a6e-106">Incident aktivnog servisa visokog prioriteta koji možda pojavljivanja.</span><span class="sxs-lookup"><span data-stu-id="52a6e-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="52a6e-107">Provjeri sve advisories/incidenata odlaskom na [Servis stanja sustava](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="52a6e-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="52a6e-108">Pomoćna automatskog popravka automatski oporavak scenarij koji nije događa zbog neočekivanih događaja na poslužiteljima koji možda zadnji za manje od 30 min ili učinili.</span><span class="sxs-lookup"><span data-stu-id="52a6e-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="52a6e-109">Postoje ne poruci centra ili servisa stanja knjiži te pomoćne recoveries, ali treba biti u običnom pogledu vrlo uskoro.</span><span class="sxs-lookup"><span data-stu-id="52a6e-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="52a6e-110">Na vrlo malo prigode smo poštovati da jedan od tri scenariji navedene su uzrok, i vratiti servisa, ali korisnici predmemorije preglednika prioritetna očišćena.</span><span class="sxs-lookup"><span data-stu-id="52a6e-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="52a6e-111">Molimo pokušaj čišćenje predmemorije preglednika prije navigacija web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="52a6e-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="52a6e-112">U pregledniku Microsoft Edge, odaberite **Postavke**, a zatim odaberite **privatnosti i sigurnosti**.</span><span class="sxs-lookup"><span data-stu-id="52a6e-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="52a6e-113">Pod **Očisti pregledavanje**, odaberite **što poništite odabir**.</span><span class="sxs-lookup"><span data-stu-id="52a6e-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="52a6e-114">Odaberite **kolačiće i podataka spremljenih web-mjesto**i odaberite **Očisti**.</span><span class="sxs-lookup"><span data-stu-id="52a6e-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="52a6e-115">Ove korake može razlikovati pri korištenju drugim preglednicima što Mozilla Firefox ili Google vizualnog.</span><span class="sxs-lookup"><span data-stu-id="52a6e-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="52a6e-116">Druga mogućnost bila bi otvorite SharePoint web-mjesta ili OneDrive u novom prozoru InPrivate.</span><span class="sxs-lookup"><span data-stu-id="52a6e-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>