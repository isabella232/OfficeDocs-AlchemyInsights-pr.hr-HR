---
title: Omogućivanje arhivskog poštanskog sandučića
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811697"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="0c05f-102">Omogućivanje arhivskog poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="0c05f-102">Enable an archive mailbox</span></span>

<span data-ttu-id="0c05f-103">Ako želite da pokrenete automatske provjere da bi se osiguralo da je moguće konfigurirati arhivski poštanski sandučić, odaberite gumb natrag < – pri vrhu ove stranice, a zatim unesite adresu e-pošte računa.</span><span class="sxs-lookup"><span data-stu-id="0c05f-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="0c05f-104">Arhivirajte poštanske sandučiće u programu Microsoft 365 (koji se nazivaju i *internetski arhivima* ili *arhivima na mjestu*) korisnicima pružite dodatnu pohranu e-pošte.</span><span class="sxs-lookup"><span data-stu-id="0c05f-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="0c05f-105">Korisnici mogu premještati ili kopirati stavke u arhivski poštanski sandučić, a administratori mogu stvarati pravilo arhiviranja koje automatski premješta stavke u arhiviranja poštanskih sandučića.</span><span class="sxs-lookup"><span data-stu-id="0c05f-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="0c05f-106">Slijede upute za stvaranje arhivskog poštanskog sandučića:</span><span class="sxs-lookup"><span data-stu-id="0c05f-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="0c05f-107">Idite na [https://protection.office.com](https://protection.office.com) .</span><span class="sxs-lookup"><span data-stu-id="0c05f-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="0c05f-108">Prijavite se u Microsoft 365 pomoću administratorskog računa.</span><span class="sxs-lookup"><span data-stu-id="0c05f-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="0c05f-109">U levom oknu centra za sigurnosno &amp; usklađivanje odaberite arhivu **upravljanja informacijama** \> **Archive**.</span><span class="sxs-lookup"><span data-stu-id="0c05f-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="0c05f-110">Odaberite korisnika čije arhivske poštanske sandučiće želite omogućiti.</span><span class="sxs-lookup"><span data-stu-id="0c05f-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="0c05f-111">U oknu s detaljima na desnoj strani kliknite **Omogući** , a zatim **da** u poruci upozorenja da biste omogućili arhivski poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="0c05f-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="0c05f-112">Arhivske poštanske sandučiće možete i masovno omogućiti tako da odaberete više korisnika (pomoću tipki **SHIFT** ili **Ctrl** ), a zatim kliknete **Omogući** u oknu s detaljima.</span><span class="sxs-lookup"><span data-stu-id="0c05f-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="0c05f-113">Zajednički poštanski sandučići</span><span class="sxs-lookup"><span data-stu-id="0c05f-113">Shared mailboxes</span></span>

<span data-ttu-id="0c05f-114">Da biste omogućili arhivu za zajednički poštanski sandučić, potrebna je licenca za tarifu sustava Exchange Online ili Exchange Online tarifa 1 s licencom za arhiviranje sustava Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="0c05f-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="0c05f-115">Da biste omogućili arhivu za zajednički poštanski sandučić, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="0c05f-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="0c05f-116">Otvorite centar za [administratore sustava Exchange](https://outlook.office365.com/ecp) i prijavite se pomoću administratorskog računa.</span><span class="sxs-lookup"><span data-stu-id="0c05f-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="0c05f-117">Idite na **Recipients**  >  **zajedničko korištenje**primatelja.</span><span class="sxs-lookup"><span data-stu-id="0c05f-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="0c05f-118">Odaberite zajednički poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="0c05f-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="0c05f-119">U oknu s detaljima na desnoj strani u odjeljku **Arhiviraj unutar mjesta**kliknite **Omogući**, a zatim **da** da biste omogućili arhivski poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="0c05f-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="0c05f-120">Dodatne informacije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="0c05f-120">For more information, see:</span></span>
  
- [<span data-ttu-id="0c05f-121">Omogućivanje arhivskih poštanskih sandučića</span><span class="sxs-lookup"><span data-stu-id="0c05f-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="0c05f-122">Postavljanje pravilnika o arhiviranju i brisanju</span><span class="sxs-lookup"><span data-stu-id="0c05f-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
