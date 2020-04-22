---
title: Premještanje poruka e-pošte u poštanski sandučić Arhive
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713638"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="2afed-102">Premještanje e-pošte u arhivski poštanski sandučić</span><span class="sxs-lookup"><span data-stu-id="2afed-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="2afed-103">Provjerite je li poštanski **sandučić arhive** omogućen.</span><span class="sxs-lookup"><span data-stu-id="2afed-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="2afed-104">Ako nije, slijedite korake u [ovom članku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) da biste omogućili poštanski sandučić arhive.</span><span class="sxs-lookup"><span data-stu-id="2afed-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="2afed-105">Da biste automatski arhivirali poruke u arhivski poštanski sandučić, oznaka zadržavanja s akcijom **Premjesti u arhivu** mora se automatski **primijeniti na cijelu oznaku poštanskog sandučića (zadano).**</span><span class="sxs-lookup"><span data-stu-id="2afed-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="2afed-106">Slijedite korake ovdje da biste izradili oznaku: [Arhiviraj zadanu oznaku](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="2afed-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="2afed-107">Zatim dodajte oznaku **Arhivu** u pravila zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="2afed-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="2afed-108">U centru za administratore sustava Exchange odaberite **Pravila zadržavanja** > **dodajte oznaku Premjesti u arhivu** u pravilo > **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="2afed-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="2afed-109">Sada [dodijelite pravila zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) poštanskom sandučiću određenog korisnika.</span><span class="sxs-lookup"><span data-stu-id="2afed-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="2afed-110">Ista pravila primijenit će se i na poštanski sandučić **Primarni** i **Arhiva.**</span><span class="sxs-lookup"><span data-stu-id="2afed-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="2afed-111">Možda će biti potrebno prisiliti pomoćnika za upravljane mape (MFA) da pokrene i primijeni nove postavke na korisnikov poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="2afed-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="2afed-112">Pokrenite sljedeću naredbu dok [ste povezani s EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli pomoćnika za upravljane mape za određeni poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="2afed-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="2afed-113">Pomoćnik za početnu mapu –identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="2afed-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="2afed-114">Dodatne informacije o postavljanju pravila arhiviranja [potražite u odjeljku Postavljanje pravila arhiviranja i brisanja za poštanske sandučiće](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="2afed-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  