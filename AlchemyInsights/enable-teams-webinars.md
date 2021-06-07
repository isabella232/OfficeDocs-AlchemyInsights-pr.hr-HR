---
title: Omogućivanje Teams web-seminara
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793548"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="de106-102">Omogućivanje Teams web-seminara</span><span class="sxs-lookup"><span data-stu-id="de106-102">Enable Teams Webinars</span></span>

<span data-ttu-id="de106-103">Web-seminari su po zadanom omogućeni.</span><span class="sxs-lookup"><span data-stu-id="de106-103">Webinars are enabled by default.</span></span> <span data-ttu-id="de106-104">Možete upravljati tko može zakazati i registrirati Teams web-seminare pomoću naredbi Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="de106-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="de106-105">Svi korisnici koji mogu stvoriti sastanak mogu stvoriti i sastanak web-seminara.</span><span class="sxs-lookup"><span data-stu-id="de106-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="de106-106">Ako želite upravljati tko može zakazati Teams, koristite *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="de106-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="de106-107">*WhoCanRegister po zadanom je* omogućen i postavljen na **Svi**.</span><span class="sxs-lookup"><span data-stu-id="de106-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="de106-108">Ako želite isključiti registraciju sastanka, *postavite AllowMeetingRegistration na* **False**.</span><span class="sxs-lookup"><span data-stu-id="de106-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="de106-109">Da biste promijenili te postavke, morate instalirati [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="de106-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="de106-110">Pravila sastanka primjenjuju se i na web-seminare Teams sastanaka.</span><span class="sxs-lookup"><span data-stu-id="de106-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="de106-111">Ako je, primjerice, anonimno uključivanje isključeno u postavkama sastanka, anonimni korisnici ne mogu se pridružiti webinarima.</span><span class="sxs-lookup"><span data-stu-id="de106-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="de106-112">Dodatne informacije o konfiguriranju osoba koje se mogu registrirati za webinare potražite u članku [Konfiguriranje osoba koje se mogu registrirati za webinare](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="de106-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="de106-113">Dodatne informacije o postavkama za Microsoftove popise potražite u članku [Postavke kontrole za Microsoftove popise](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="de106-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>