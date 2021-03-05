---
title: Saznajte tko je postavio prosljeđivanje na poštanskom sandučiću i kako
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481204"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="15032-102">Saznajte tko je postavio prosljeđivanje na poštanskom sandučiću i kako</span><span class="sxs-lookup"><span data-stu-id="15032-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="15032-103">Ako je vanjsko prosljeđivanje postavljeno na poštanski sandučić, aktivnost se nadzire kao dio cmdleta Set-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="15032-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="15032-104">Slijede upute za pronalaženje aktivnosti u zapisniku nadzora:</span><span class="sxs-lookup"><span data-stu-id="15032-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="15032-105">Otvorite centar za [sigurnost & sustava Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="15032-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="15032-106">Odaberite **Pretraži pretragu** >  **zapisnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="15032-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="15032-107">Ako vam se prikaže obavijest da morate uključiti nadzor, nastavite i uključite ga odmah.</span><span class="sxs-lookup"><span data-stu-id="15032-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="15032-108">Ako ta značajka nije uključena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.</span><span class="sxs-lookup"><span data-stu-id="15032-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="15032-109">Provjerite je li polje **aktivnosti** postavljeno tako da **prikazuje rezultate za sve aktivnosti** (zadano).</span><span class="sxs-lookup"><span data-stu-id="15032-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="15032-110">Navedite raspon datuma.</span><span class="sxs-lookup"><span data-stu-id="15032-110">Specify the date range.</span></span> <span data-ttu-id="15032-111">Ne morate navesti korisničko ime.</span><span class="sxs-lookup"><span data-stu-id="15032-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="15032-112">Odaberite **Pretraživanje**.</span><span class="sxs-lookup"><span data-stu-id="15032-112">Select **Search**.</span></span> <span data-ttu-id="15032-113">Aktivnosti se prikazuju u odjeljku **Rezultati**.</span><span class="sxs-lookup"><span data-stu-id="15032-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="15032-114">Odaberite **Filtriraj rezultate**, a zatim u polje Filtar **aktivnosti** unesite **skup poštanskih sandučića** .</span><span class="sxs-lookup"><span data-stu-id="15032-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="15032-115">Time se vraća sve aktivnosti **skupa poštanskih sandučića** .</span><span class="sxs-lookup"><span data-stu-id="15032-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="15032-116">Da biste pogledali detalje, odaberite aktivnost, a zatim odaberite **Dodatne informacije**.</span><span class="sxs-lookup"><span data-stu-id="15032-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="15032-117">U odjeljku **Parametri** možete vidjeti adresu e-pošte za prosljeđivanje koja je postavljena na poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="15032-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="15032-118">**Userid** predstavlja korisnika koji je postavio vanjsko prosljeđivanje na poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="15032-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="15032-119">Dodatne informacije potražite u članku [pretraživanje zapisnika nadzora sustava Office 365 radi otklanjanja običnih scenarija](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="15032-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>