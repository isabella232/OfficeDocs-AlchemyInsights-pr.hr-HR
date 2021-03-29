---
title: Provjera prosljeđivanja adresa u poštanskim sandučićima
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403303"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="6e4ff-102">Provjera prosljeđivanja adresa u poštanskim sandučićima</span><span class="sxs-lookup"><span data-stu-id="6e4ff-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="6e4ff-103">Hakeri katkad prosljeđuju poruke e-pošte korisnicima, pa ćemo najprije provjeriti ima li adresa i pravila u poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="6e4ff-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="6e4ff-104">Zatim ćemo provjeriti zapisnike nadzora.</span><span class="sxs-lookup"><span data-stu-id="6e4ff-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="6e4ff-105">Evo kako provjeriti ima li adresa za prosljeđivanje:</span><span class="sxs-lookup"><span data-stu-id="6e4ff-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="6e4ff-106">Odaberite **Korisnici**  >  **Aktivni korisnici**.</span><span class="sxs-lookup"><span data-stu-id="6e4ff-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="6e4ff-107">Odaberite korisnika čiji je račun ugrožen.</span><span class="sxs-lookup"><span data-stu-id="6e4ff-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="6e4ff-108">U podlošci koji će se prikazati proširite **Odjeljak Postavke pošte**, a zatim kliknite Uređivanje **za** prosljeđivanje **e-pošte**.</span><span class="sxs-lookup"><span data-stu-id="6e4ff-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="6e4ff-109">Uklonite sve adrese za prosljeđivanje koje ne prepoznajete.</span><span class="sxs-lookup"><span data-stu-id="6e4ff-109">Remove any forwarding addresses you don't recognize.</span></span>