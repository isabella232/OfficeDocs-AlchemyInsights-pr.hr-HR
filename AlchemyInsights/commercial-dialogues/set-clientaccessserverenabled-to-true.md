---
title: Postavljanje značajke ClientAccessServerEnabled u True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743771"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="43ba4-102">Postavljanje značajke ClientAccessServerEnabled u True</span><span class="sxs-lookup"><span data-stu-id="43ba4-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="43ba4-103">Ako ne možete otvoriti šifriranu poruku e-pošte i umjesto njega vidjeti privitak s **rpmsg** -a, slijedite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="43ba4-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="43ba4-104">Spojite se na PowerShell sustava Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="43ba4-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="43ba4-105">Da biste se povezali sa komponenti Exchange Online PowerShell, morate se prijaviti pomoću globalnog administratora ili administratora za administratore sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="43ba4-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="43ba4-106">je.</span><span class="sxs-lookup"><span data-stu-id="43ba4-106">a.</span></span> <span data-ttu-id="43ba4-107">Otvorite Windows PowerShell, a zatim pokrenite sljedeću naredbu: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="43ba4-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="43ba4-108">b.</span><span class="sxs-lookup"><span data-stu-id="43ba4-108">b.</span></span> <span data-ttu-id="43ba4-109">U dijaloškom okviru **zahtjev za vjerodajnice vjerodajnica za Windows PowerShell** unesite svoj račun za rad ili školovanje i lozinku, c.</span><span class="sxs-lookup"><span data-stu-id="43ba4-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="43ba4-110">Kliknite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="43ba4-110">Click **OK**.</span></span> 

2. <span data-ttu-id="43ba4-111">Pokrenite sljedeću naredbu da biste stvorili novu sesiju:</span><span class="sxs-lookup"><span data-stu-id="43ba4-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="43ba4-112">je.</span><span class="sxs-lookup"><span data-stu-id="43ba4-112">a.</span></span> <span data-ttu-id="43ba4-113">Izvršite sljedeću naredbu:</span><span class="sxs-lookup"><span data-stu-id="43ba4-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="43ba4-114">Pokreni `Get-IRMConfiguration` naredbu.</span><span class="sxs-lookup"><span data-stu-id="43ba4-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="43ba4-115">Provjerite postavku **Clientaccessserverenabled** .</span><span class="sxs-lookup"><span data-stu-id="43ba4-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="43ba4-116">je.</span><span class="sxs-lookup"><span data-stu-id="43ba4-116">a.</span></span> <span data-ttu-id="43ba4-117">Ako je postavka **Clientaccessserverenabled** postavljena na **False**, pokrenite sljedeći cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="43ba4-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="43ba4-118">Uvijek zatvarate sesiju PowerShell uz sljedeću naredbu: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="43ba4-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="43ba4-119">Dodatne informacije potražite u članku [Microsoft Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="43ba4-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

