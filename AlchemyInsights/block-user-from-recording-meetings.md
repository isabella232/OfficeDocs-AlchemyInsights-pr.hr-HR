---
title: Blokiranje korisnika u snimanju sastanaka
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035056"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="f9f9d-102">Blokiranje korisnika u snimanju sastanaka</span><span class="sxs-lookup"><span data-stu-id="f9f9d-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="f9f9d-103">Ako morate **spriječiti ili blokirati** određene korisnike na sastancima timova, to možete učiniti putem postavki pravilnika za sastanke u timovima.</span><span class="sxs-lookup"><span data-stu-id="f9f9d-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="f9f9d-104">U centru za administratore Microsoft timova isključite postavku **Dopusti snimanje oblaka** u pravilima sastanka dodijeljenim tom korisniku.</span><span class="sxs-lookup"><span data-stu-id="f9f9d-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="f9f9d-105">Dodatne informacije potražite u članku [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span><span class="sxs-lookup"><span data-stu-id="f9f9d-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="f9f9d-106">Da biste provjerili je li određeni korisnik dopušten ili nije za snimanje sastanaka timova, upotrijebite dijagnostički alat za podršku.</span><span class="sxs-lookup"><span data-stu-id="f9f9d-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="f9f9d-107">Pokrenite novi upit za podršku i upišite u **dijag: snimanje sastanka** – dijagnostički će provjeriti postavke pravilnika za određenog korisnika i odrediti njihove postavke pravilnika.</span><span class="sxs-lookup"><span data-stu-id="f9f9d-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="f9f9d-108">Zapamtite, za nove postavke pravilnika može potrajati nekoliko sati, pa ako ste upravo unijeli promjenu, pričekajte nekoliko sati prije ponovnog pokretanja dijagnostike.</span><span class="sxs-lookup"><span data-stu-id="f9f9d-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="f9f9d-109">Dodatne informacije potražite u odjeljku [Uključivanje ili isključivanje snimanja oblaka](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span><span class="sxs-lookup"><span data-stu-id="f9f9d-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
