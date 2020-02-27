---
title: Izradite e-mail catch sve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286061"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="ada7e-102">Izradite e-mail catch sve</span><span class="sxs-lookup"><span data-stu-id="ada7e-102">Create an email catch all</span></span>

<span data-ttu-id="ada7e-103">Korištenje ulova sve je snažno obeshrabreno.</span><span class="sxs-lookup"><span data-stu-id="ada7e-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="ada7e-104">Bolje je pružiti povrat natrag pošiljatelju ostavljajući pošiljateljima do znanja da se njihova poruka ne može isporučiti kako bi mogli poduzeti radnje.</span><span class="sxs-lookup"><span data-stu-id="ada7e-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="ada7e-105">Nadzirani poštanski sandučić možete ograničiti i tako da uhvati samo ranije valjane adrese e-pošte.</span><span class="sxs-lookup"><span data-stu-id="ada7e-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="ada7e-106">Svaki ulov sve poštanski sandučić će dobiti mnogo spam i svibanj na kraju ispuniti ako ne i pomno pratiti.</span><span class="sxs-lookup"><span data-stu-id="ada7e-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="ada7e-107">(Postoje ograničenja primanja.)</span><span class="sxs-lookup"><span data-stu-id="ada7e-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="ada7e-108">Ako odlučite nastaviti, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="ada7e-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="ada7e-109">Stvaranje grupe za dinamičku raspodjelu & uključuju "Sve vrste primatelja".</span><span class="sxs-lookup"><span data-stu-id="ada7e-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="ada7e-110">Izradite namjenski poštanski sandučić za ulak za e-poštu, na primjer catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="ada7e-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="ada7e-111">Za određenu domenu postavite DomainType na "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="ada7e-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="ada7e-112">Ako kasnije uklonite ulov sve, budite sigurni da postavite domenu natrag na autoritativno.</span><span class="sxs-lookup"><span data-stu-id="ada7e-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="ada7e-113">Kreirajte pravilo prijenosa tijeka pošte na sljedeći način:</span><span class="sxs-lookup"><span data-stu-id="ada7e-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="ada7e-114">Ako je pošiljatelj "Izvan organizacije"</span><span class="sxs-lookup"><span data-stu-id="ada7e-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="ada7e-115">Preusmjeravanje poruke na Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="ada7e-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="ada7e-116">Osim ako je primatelj član allusers@domain.com (Grupa raspodjele sadrži sve članove)</span><span class="sxs-lookup"><span data-stu-id="ada7e-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="ada7e-117">Provjera valjanosti dodavanja novih poštanskih sandučića u grupu za dinamičku raspodjelu</span><span class="sxs-lookup"><span data-stu-id="ada7e-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
