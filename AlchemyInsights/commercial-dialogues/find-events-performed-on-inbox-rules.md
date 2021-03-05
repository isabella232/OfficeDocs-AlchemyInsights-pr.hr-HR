---
title: Pronalaženje događaja izvedenih u pravilima ulazne pošte
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481276"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="506a4-102">Pronalaženje događaja izvedenih u pravilima ulazne pošte</span><span class="sxs-lookup"><span data-stu-id="506a4-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="506a4-103">Kada se pravila ulazne pošte stvaraju, mijenjaju ili brišu, događaji se snimaju u zapisniku nadzora.</span><span class="sxs-lookup"><span data-stu-id="506a4-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="506a4-104">Slijede upute za pregled:</span><span class="sxs-lookup"><span data-stu-id="506a4-104">Here's how to review them:</span></span>

1. <span data-ttu-id="506a4-105">Otvorite centar za [sigurnost & sustava Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="506a4-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="506a4-106">Odaberite Pretraži > pretraživanju zapisnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="506a4-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="506a4-107">Ako vam se prikaže obavijest da morate uključiti nadzor, nastavite i uključite ga odmah.</span><span class="sxs-lookup"><span data-stu-id="506a4-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="506a4-108">Ako ta značajka nije uključena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.</span><span class="sxs-lookup"><span data-stu-id="506a4-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="506a4-109">Odaberite polje aktivnosti i pronađite aktivnosti poštanskog sandučića sustava Exchange, a zatim odaberite New-InboxRule Stvori pravilo ulazne pošte iz web-aplikacije Outlook e.</span><span class="sxs-lookup"><span data-stu-id="506a4-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="506a4-110">Kada završite, kliknite izvan okna da biste minimizirali okno aktivnosti.</span><span class="sxs-lookup"><span data-stu-id="506a4-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="506a4-111">Navedite raspon datuma, a zatim u polju korisnici odaberite korisničko ime za korisnika koje želite istražiti.</span><span class="sxs-lookup"><span data-stu-id="506a4-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="506a4-112">Možete odabrati više korisnika istodobno.</span><span class="sxs-lookup"><span data-stu-id="506a4-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="506a4-113">Odaberite pretraživanje.</span><span class="sxs-lookup"><span data-stu-id="506a4-113">Select Search.</span></span> <span data-ttu-id="506a4-114">Aktivnosti se prikazuju u odjeljku Rezultati.</span><span class="sxs-lookup"><span data-stu-id="506a4-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="506a4-115">Da biste pogledali detalje, odaberite aktivnost, a zatim odaberite dodatne informacije.</span><span class="sxs-lookup"><span data-stu-id="506a4-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="506a4-116">U odjeljku parametri možete vidjeti naziv pravila, uvjeti postavljeni i akcije koje će pravilo poduzeti.</span><span class="sxs-lookup"><span data-stu-id="506a4-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="506a4-117">Dodatne informacije potražite u članku pretraživanje zapisnika nadzora sustava Office 365 radi otklanjanja običnih scenarija.</span><span class="sxs-lookup"><span data-stu-id="506a4-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>