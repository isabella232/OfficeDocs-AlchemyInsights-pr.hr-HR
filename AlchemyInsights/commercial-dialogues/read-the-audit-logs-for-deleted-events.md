---
title: Čitanje zapisnika nadzora za izbrisane događaje
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481196"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="4654e-102">Čitanje zapisnika nadzora za izbrisane događaje</span><span class="sxs-lookup"><span data-stu-id="4654e-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="4654e-103">Evo kako to učiniti:</span><span class="sxs-lookup"><span data-stu-id="4654e-103">Here's how to do this:</span></span>

1. <span data-ttu-id="4654e-104">Otvorite centar za [sigurnost & sustava Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="4654e-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="4654e-105">Odaberite **Pretraži pretragu**  >  [**zapisnika nadzora**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="4654e-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="4654e-106">Ako vam se prikaže obavijest da je potrebno uključiti značajku, nastavite i uključite je sada.</span><span class="sxs-lookup"><span data-stu-id="4654e-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="4654e-107">Ako značajka nije uključena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.</span><span class="sxs-lookup"><span data-stu-id="4654e-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="4654e-108">Odaberite **aktivnosti**, a zatim pronađite **aktivnosti poštanskog sandučića sustava Exchange**.</span><span class="sxs-lookup"><span data-stu-id="4654e-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="4654e-109">Odaberite **izbrisane poruke iz mape Izbrisane stavke** i **premjestite poruke u mogućnosti mape Izbrisane stavke** .</span><span class="sxs-lookup"><span data-stu-id="4654e-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="4654e-110">Kada završite, kliknite izvan okna da biste minimizirali okno **aktivnosti** .</span><span class="sxs-lookup"><span data-stu-id="4654e-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="4654e-111">Navedite raspon datuma, a zatim u okviru **korisnici** odaberite korisničko ime za korisnika koje želite istražiti.</span><span class="sxs-lookup"><span data-stu-id="4654e-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="4654e-112">Možete odabrati više korisnika istodobno.</span><span class="sxs-lookup"><span data-stu-id="4654e-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="4654e-113">Odaberite **Pretraživanje**.</span><span class="sxs-lookup"><span data-stu-id="4654e-113">Select **Search**.</span></span> <span data-ttu-id="4654e-114">Aktivnosti se prikazuju u odjeljku **Rezultati**.</span><span class="sxs-lookup"><span data-stu-id="4654e-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="4654e-115">Da biste pogledali detalje, odaberite aktivnost, a zatim odaberite **Dodatne informacije**.</span><span class="sxs-lookup"><span data-stu-id="4654e-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="4654e-116">Dodatne informacije o izbrisanoj stavci, kao što su redak predmeta i mjesto stavke kada je izbrisana, prikazat će se u polju **Afecteditems** .</span><span class="sxs-lookup"><span data-stu-id="4654e-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="4654e-117">Izbrisane stavke ne možete vratiti pomoću značajke zapisnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="4654e-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="4654e-118">Da biste vratili izbrisane stavke, pročitajte članak [obnova izbrisanih stavki ili e-pošte u web-aplikaciji Outlook](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="4654e-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="4654e-119">Dodatne informacije potražite u članku [pretraživanje zapisnika nadzora sustava Office 365 radi otklanjanja običnih scenarija](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="4654e-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
