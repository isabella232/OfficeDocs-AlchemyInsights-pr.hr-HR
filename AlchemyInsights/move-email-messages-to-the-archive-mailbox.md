---
title: Premještanje poruka e-pošte u poštanski sandučić Arhiva
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
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522763"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="1736d-102">Premještanje e-pošte u poštanski sandučić arhive</span><span class="sxs-lookup"><span data-stu-id="1736d-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="1736d-103">Ako želite da pokrenemo automatske provjere za postavke navedene u nastavku, odaberite gumb natrag <-- pri vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema s premještanjem e-pošte u svoj arhivski poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="1736d-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="1736d-104">Provjerite je li omogućen **poštanski sandučić arhive.**</span><span class="sxs-lookup"><span data-stu-id="1736d-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="1736d-105">Ako nije, pomoću koraka u [ovom članku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) omogućite poštanski sandučić arhive.</span><span class="sxs-lookup"><span data-stu-id="1736d-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="1736d-106">Da bi se poruke automatski arhivirale u poštanski sandučić arhive, oznaka zadržavanja s akcijom **Premjesti u arhiv** mora biti postavljena tako da se automatski primjenjuje na cijeli poštanski sandučić **(zadana) oznaka**.</span><span class="sxs-lookup"><span data-stu-id="1736d-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="1736d-107">Slijedite korake ovdje da biste izradili oznaku: [Arhiviraj zadanu oznaku](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="1736d-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="1736d-108">Zatim dodajte oznaku **Arhiva** u pravila zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="1736d-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="1736d-109">U centru za administratore sustava Exchange odaberite **Pravila zadržavanja** > dodati **oznaku Premjesti** u arhivu u pravila > **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="1736d-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="1736d-110">Sada [dodijelite pravila zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) određenom korisničkom poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="1736d-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="1736d-111">Ista pravila primijenit će se i na poštanski sandučić **Primarna** i **arhiva.**</span><span class="sxs-lookup"><span data-stu-id="1736d-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="1736d-112">Možda će biti potrebno prisiliti pomoćnika za upravljane mape (MFA) da pokrene i primijeni nove postavke na poštanski sandučić korisnika.</span><span class="sxs-lookup"><span data-stu-id="1736d-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="1736d-113">Pokrenite sljedeću naredbu dok [ste povezani s exo powershellom da](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) biste pokrenuli pomoćnika za upravljane mape za određeni poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="1736d-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="1736d-114">Početni upravljani identitet pomoćnika -identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="1736d-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="1736d-115">Dodatne informacije o postavljanju pravila arhiviranja potražite [u odjeljku Postavljanje pravila arhiviranja i brisanja poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="1736d-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  