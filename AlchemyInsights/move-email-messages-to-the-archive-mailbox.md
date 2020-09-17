---
title: Premještanje poruka e-pošte u arhivski poštanski sandučić
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799772"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="b94b4-102">Premještanje e-pošte u arhivski poštanski sandučić</span><span class="sxs-lookup"><span data-stu-id="b94b4-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="b94b4-103">Ako želite da pokrenete automatske provjere za navedene postavke, odaberite gumb natrag < – pri vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema s premještanjem e-pošte u arhivski poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="b94b4-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="b94b4-104">Potvrdite da je omogućen **arhivski poštanski sandučić** .</span><span class="sxs-lookup"><span data-stu-id="b94b4-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="b94b4-105">Ako ne, slijedite upute u [ovom članku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) da biste omogućili arhivski poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="b94b4-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="b94b4-106">Da biste automatski arhivirali poruke u arhivski poštanski sandučić, oznaka zadržavanja s akcijom **Premjesti u arhiviranje** mora biti postavljena tako da se **automatski primjenjuje na cijeli poštanski sandučić (zadana) oznaka**.</span><span class="sxs-lookup"><span data-stu-id="b94b4-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="b94b4-107">Koristite korake ovdje da biste stvorili oznaku: [Arhiviraj zadanu oznaku](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="b94b4-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="b94b4-108">Zatim dodajte oznaku **arhive** u pravilnik o zadržavanju.</span><span class="sxs-lookup"><span data-stu-id="b94b4-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="b94b4-109">U centru za administratore sustava Exchange odaberite **pravila zadržavanja** > Dodajte **oznaku Premjesti u arhivu** da bi se pravila > **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="b94b4-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="b94b4-110">Sada [dodijelite pravilnik o zadržavanju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) za poštanski sandučić određenog korisnika.</span><span class="sxs-lookup"><span data-stu-id="b94b4-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="b94b4-111">Isto pravilo primijenit će se i na **primarni** i **arhivski** poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="b94b4-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="b94b4-112">Možda će biti potrebno prisiliti pomoćnika za upravljanu mapu (MFA) da pokreće i Primijeni nove postavke na korisnikov poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="b94b4-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="b94b4-113">Pokrenite sljedeću naredbu dok ste [povezani s programom EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli pomoćnik za upravljane mape za određeni poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="b94b4-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="b94b4-114">Start-ManagedFolderAssistant-Identity <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="b94b4-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="b94b4-115">Dodatne informacije o postavljanju pravilnika arhiviranja potražite [u članku Postavljanje pravilnika o arhiviranju i brisanju za poštanske sandučiće](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="b94b4-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  