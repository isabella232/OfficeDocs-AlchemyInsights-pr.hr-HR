---
title: Upravljanje registracijom webinara
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793617"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="ecb28-102">Upravljanje registracijom webinara</span><span class="sxs-lookup"><span data-stu-id="ecb28-102">Manage webinar registration</span></span>

<span data-ttu-id="ecb28-103">Upravljate tko se može registrirati za Teams web-seminare pomoću Teams powershell naredbi.</span><span class="sxs-lookup"><span data-stu-id="ecb28-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="ecb28-104">Da biste instalirali Teams PowerShell, [pogledajte Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="ecb28-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="ecb28-105">*WhoCanRegister po zadanom je* omogućen i postavljen na **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="ecb28-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="ecb28-106">Da biste svima, uključujući anonimne korisnike, omogućili registraciju, morate postaviti pravilnik sastanka **svima** pomoću naredbe Powershell:</span><span class="sxs-lookup"><span data-stu-id="ecb28-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="ecb28-107">**Napomena:** ako je anonimno pridruživanje isključeno u postavkama sastanka, anonimni korisnici ne mogu se uključiti u web-seminare.</span><span class="sxs-lookup"><span data-stu-id="ecb28-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="ecb28-108">Dodatne informacije i omogućivanje te postavke potražite u članku [Upravljanje postavkama sastanka Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ecb28-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="ecb28-109">Ako želite isključiti registraciju sastanka, *postavite AllowMeetingRegistration na* **False**.</span><span class="sxs-lookup"><span data-stu-id="ecb28-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="ecb28-110">Dodatne informacije o konfiguriranju osoba koje se mogu registrirati za webinare potražite u članku [Konfiguriranje osoba koje se mogu registrirati za webinare](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="ecb28-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="ecb28-111">Dodatne informacije o postavkama za Microsoftove popise potražite u članku [Postavke kontrole za Microsoftove popise](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="ecb28-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
