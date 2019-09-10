---
title: Premještanje poruka e-pošte u poštanski sandučić arhive
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822154"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="a371f-102">Premještanje e-pošte u poštanski sandučić arhive</span><span class="sxs-lookup"><span data-stu-id="a371f-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="a371f-103">Provjerite je li omogućen **Poštanski sandučić arhive** .</span><span class="sxs-lookup"><span data-stu-id="a371f-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="a371f-104">Ako ne, koristite korake u [ovom članku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) da biste omogućili arhiviranje poštanskog sandučića.</span><span class="sxs-lookup"><span data-stu-id="a371f-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="a371f-105">Da biste automatski arhivirali poruke u poštanski sandučić arhive, oznaka zadržavanja s **premještavanjem u arhivsku** akciju mora biti postavljena da se **automatski primijeni na cijelu oznaku poštanskog sandučića (zadana)**.</span><span class="sxs-lookup"><span data-stu-id="a371f-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="a371f-106">Pomoću koraka ovdje stvorite oznaku: [arhivirati zadanu oznaku](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="a371f-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="a371f-107">Zatim u pravila zadržavanja dodajte oznaku **arhive** .</span><span class="sxs-lookup"><span data-stu-id="a371f-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="a371f-108">U centru za administratore sustava Exchange odaberite **pravila zadržavanja** > Dodajte **oznaku Premjesti u arhivu** pravila > **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="a371f-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="a371f-109">Sada [dodijelite pravila zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) određenom korisnikovom poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="a371f-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="a371f-110">Isto pravilo će se primijeniti i na **primarni** i **Arhiva** poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="a371f-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="a371f-111">Možda će biti potrebno prisiliti pomoćnika za upravljane mape (MFA) da radi i Primijeni nove postavke na korisnički poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="a371f-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="a371f-112">Pokrenite sljedeću naredbu dok ste [spojeni na EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli upravljani pomoćnik mape za određeni poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="a371f-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="a371f-113">Start-ManagedFolderAssistant-identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="a371f-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="a371f-114">Za više informacija o postavljanju pravila arhive, pogledajte [Postavljanje pravila arhive i brisanja za poštanske sandučiće](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="a371f-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  