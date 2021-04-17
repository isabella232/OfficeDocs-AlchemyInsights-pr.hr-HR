---
title: Stvaranje ulova e-pošte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816192"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="6c415-102">Stvaranje ulova e-pošte</span><span class="sxs-lookup"><span data-stu-id="6c415-102">Create an email catch all</span></span>

<span data-ttu-id="6c415-103">Korištenje ulova sve je jako obeshrabreno.</span><span class="sxs-lookup"><span data-stu-id="6c415-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="6c415-104">Bolje je vratiti pošiljatelja da zna da se njihova poruka ne može isporučiti kao adresa da bi mogli poduzeti akciju.</span><span class="sxs-lookup"><span data-stu-id="6c415-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="6c415-105">Možete i ograničiti nadzirani poštanski sandučić tako da ulovi samo prijašnje valjane adrese e-pošte.</span><span class="sxs-lookup"><span data-stu-id="6c415-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="6c415-106">Svaki ulov svih poštanskih sandučića primit će mnogo neželjene pošte i naposljetku će se možda popuniti ako se ne nadzire.</span><span class="sxs-lookup"><span data-stu-id="6c415-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="6c415-107">(Postoje ograničenja primanja.)</span><span class="sxs-lookup"><span data-stu-id="6c415-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="6c415-108">Ako odlučite nastaviti, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="6c415-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="6c415-109">Stvaranje grupe za dinamičku raspodjelu & "Sve vrste primatelja".</span><span class="sxs-lookup"><span data-stu-id="6c415-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="6c415-110">Stvorite namjenski poštanski sandučić da biste uhvatili poruke e-pošte, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="6c415-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="6c415-111">Za određenu domenu postavite DomainType na "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="6c415-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="6c415-112">Ako kasnije uklonite sve ulov, obavezno vratite domenu na Mjerodavno.</span><span class="sxs-lookup"><span data-stu-id="6c415-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="6c415-113">Stvorite pravilo prijenosa tijeka pošte na sljedeći način:</span><span class="sxs-lookup"><span data-stu-id="6c415-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="6c415-114">Ako je pošiljatelj "Outside the Organization" (Izvan tvrtke ili ustanove)</span><span class="sxs-lookup"><span data-stu-id="6c415-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="6c415-115">Preusmjeravanje poruke na Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="6c415-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="6c415-116">Osim ako je primatelj član grupe allusers@domain.com (grupa za raspodjelu sadrži sve članove)</span><span class="sxs-lookup"><span data-stu-id="6c415-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="6c415-117">Provjerite jesu li novi poštanski sandučići dodani u grupu za dinamičku raspodjelu</span><span class="sxs-lookup"><span data-stu-id="6c415-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
