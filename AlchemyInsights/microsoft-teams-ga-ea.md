---
title: Microsoftovi timovi – pristup gostu
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: da9ecca062bd5f1dcc169657483ba53eb201def0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798368"
---
# <a name="microsoft-teams---guest-access"></a><span data-ttu-id="98398-102">Microsoftovi timovi – pristup gostu</span><span class="sxs-lookup"><span data-stu-id="98398-102">Microsoft Teams - Guest Access</span></span>

<span data-ttu-id="98398-103">Ako vam je potrebna pomoć u komunikaciji s korisnicima izvan tvrtke ili ustanove u timovima, morate odlučiti želite li koristiti [pristup gostu ili vanjski pristup (Federaciju)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)ili možete koristiti oba.</span><span class="sxs-lookup"><span data-stu-id="98398-103">If you need help communicating with users outside your Organization in Teams, you need to decide whether to use [Guest Access or External Access (Federation)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access), or you can use both.</span></span>

<span data-ttu-id="98398-104">Obavezno [Pregledajte razlike](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) da biste razumjeli značajke koje su dostupne za svaku od njih.</span><span class="sxs-lookup"><span data-stu-id="98398-104">Be sure to [review the differences](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) to understand the features available for each.</span></span>  <span data-ttu-id="98398-105">Na primjer, vanjski pristup (Federacija) dopušta 1:1 komunikacija, kao što su čavrljanje i prisutnost.</span><span class="sxs-lookup"><span data-stu-id="98398-105">For example, External access (federation) allows for 1:1 communications, like Chat and Presence.</span></span>  <span data-ttu-id="98398-106">Udruženim korisnicima nije moguće sudjelovati u suradnji timova.</span><span class="sxs-lookup"><span data-stu-id="98398-106">Federated users cannot participate in Teams collaboration however.</span></span>  <span data-ttu-id="98398-107">Ako želite da se vanjski korisnik pridruži i sudjeluje u razgovorima s timovima ili zajednički koristi datoteke, morat ćete uključiti pristup gostu.</span><span class="sxs-lookup"><span data-stu-id="98398-107">If you’d like an external user to join and participate in Teams Channel Conversations or Share Files, you’ll need to turn on Guest Access.</span></span>

<span data-ttu-id="98398-108">**Prva mogućnost: uključivanje pristupa gostu** </span><span class="sxs-lookup"><span data-stu-id="98398-108">**Option 1: Turn on Guest Access** </span></span>  
<span data-ttu-id="98398-109">U centru za administratore timova idite na web-mjesta [org Wide postavke > pristup gostu](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) i uključite "Dopusti gostu pristup u timovima".</span><span class="sxs-lookup"><span data-stu-id="98398-109">In the Teams Admin Center, Go to [Org Wide Settings > Guest Access](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) and turn on “Allow Guest Access in Teams”.</span></span>  <span data-ttu-id="98398-110">Za zakupca sa svim ostalim zadanim postavkama to bi trebalo biti sve što trebate učiniti.</span><span class="sxs-lookup"><span data-stu-id="98398-110">For a tenant with all other default settings, this should be all you need to do.</span></span>  <span data-ttu-id="98398-111">Da biste prilagodili konfiguraciju pristupa gostu, obavezno slijedite sve korake u [kontrolnom popisu pristup gostu](https://docs.microsoft.com/microsoftteams/guest-access-checklist).</span><span class="sxs-lookup"><span data-stu-id="98398-111">To customize your Guest Access configuration,  make sure you follow all the steps in the [Guest Access Checklist](https://docs.microsoft.com/microsoftteams/guest-access-checklist).</span></span> <span data-ttu-id="98398-112">Kada završite s potpunim, morat ćete [čekati do 24 sata](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) da postavke stupite na utjecaj.</span><span class="sxs-lookup"><span data-stu-id="98398-112">Once you're completely done, you'll need to [wait up to 24 hours](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) for the settings to take effect.</span></span>

<span data-ttu-id="98398-113">Ako ste sigurni da ste dovršili sve korake na popisu, a prošlo je više od 24 sata, nastavite i pokušajte [dodati gosta u svoj tim](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).</span><span class="sxs-lookup"><span data-stu-id="98398-113">If you’re confident you’ve completed all the steps in the Checklist, and it's been more than 24 hours, go ahead and try to [add a Guest to your Team](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).</span></span>

<span data-ttu-id="98398-114">Dodatne informacije, uključujući videozapise s načinom na koji se prikazuje, potražite [u članku pristup gostu u Microsoftovim timovima](https://docs.microsoft.com/microsoftteams/guest-access).</span><span class="sxs-lookup"><span data-stu-id="98398-114">For more information, including how-to videos, see [Guest access in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).</span></span>

<span data-ttu-id="98398-115">Druga **mogućnost: uključivanje vanjskog pristupa (Federacija)** Ako želite uključiti i vanjski pristup (Federacija), u centru za administratore timova idite na [Postavke sustava > vanjski pristup](https://admin.teams.microsoft.com/company-wide-settings/external-communications) , a zatim uključite "korisnici mogu komunicirati s korisnicima Skypea za tvrtke i timove", a zatim slijedite sve korake u odjeljku [Dopusti korisnicima da čavrljamo i komunicirajte s korisnicima u drugoj tvrtki ili ustanovi](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).</span><span class="sxs-lookup"><span data-stu-id="98398-115">**Option 2: Turn On External Access (Federation)** If you’d also like to turn on External Access (Federation), in the Teams Admin center go to [Org-wide Settings > External Access](https://admin.teams.microsoft.com/company-wide-settings/external-communications) and turn on "Users can communicate with Skype for Business and Teams users", and then follow all the steps in [Let your Teams users chat and communicate with users in another organization](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).</span></span>


