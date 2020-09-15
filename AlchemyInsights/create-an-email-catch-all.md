---
title: Stvaranje e-pošte za hvatanje svih
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712978"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="04a65-102">Stvaranje e-pošte za hvatanje svih</span><span class="sxs-lookup"><span data-stu-id="04a65-102">Create an email catch all</span></span>

<span data-ttu-id="04a65-103">Korištenje hvatanja sve se snažno obeshrabri.</span><span class="sxs-lookup"><span data-stu-id="04a65-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="04a65-104">Bolje je vratiti pošiljatelju da pošalje pošiljatelja da zna da se poruka ne može isporučiti kao adresirana da bi mogla poduzeti akcije.</span><span class="sxs-lookup"><span data-stu-id="04a65-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="04a65-105">Možete i ograničiti nadzirani poštanski sandučić samo da biste uhvatili prethodno valjane adrese e-pošte.</span><span class="sxs-lookup"><span data-stu-id="04a65-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="04a65-106">Bilo koji ulov svi poštanski sandučić dobit će dobar dio neželjene pošte i eventualno može popuniti ako ne pomno prati.</span><span class="sxs-lookup"><span data-stu-id="04a65-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="04a65-107">(Postoje ograničenja koja primate)</span><span class="sxs-lookup"><span data-stu-id="04a65-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="04a65-108">Ako odlučite nastaviti, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="04a65-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="04a65-109">Stvaranje grupe za dinamičku raspodjelu & obuhvaća "sve vrste primatelja".</span><span class="sxs-lookup"><span data-stu-id="04a65-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="04a65-110">Stvorite namjenski poštanski sandučić da biste uhvatili poruke e-pošte, primjerice catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="04a65-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="04a65-111">Za određene domene postavite domenu domena na "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="04a65-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="04a65-112">Ako kasnije uklonite sve nalaze, obavezno ponovno postavite domenu na autoritativno.</span><span class="sxs-lookup"><span data-stu-id="04a65-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="04a65-113">Stvaranje pravila transporta e-pošte na sljedeći način:</span><span class="sxs-lookup"><span data-stu-id="04a65-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="04a65-114">Ako je pošiljatelj "izvan tvrtke ili ustanove"</span><span class="sxs-lookup"><span data-stu-id="04a65-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="04a65-115">Preusmjeravanje poruke na Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="04a65-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="04a65-116">Osim ako je primatelj član allusers@domain.com (grupa za raspodjelu sadrži sve članove)</span><span class="sxs-lookup"><span data-stu-id="04a65-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="04a65-117">Provjerite jeste li potvrdili da se novi poštanski sandučići dodaju u grupu za dinamičku raspodjelu</span><span class="sxs-lookup"><span data-stu-id="04a65-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
