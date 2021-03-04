---
title: Provjera prosljeđivanja adresa na poštanskim sandučićima
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427130"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="4e3d1-102">Provjera prosljeđivanja adresa na poštanskim sandučićima</span><span class="sxs-lookup"><span data-stu-id="4e3d1-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="4e3d1-103">Ponekad hakeri prosljeđuju poruke e-pošte korisnika sami sebi, pa ćemo najprije provjeriti ima li adresa i pravila za prosljeđivanje na poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="4e3d1-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="4e3d1-104">Onda ćemo provjeriti evidencije nadzora.</span><span class="sxs-lookup"><span data-stu-id="4e3d1-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="4e3d1-105">Slijede upute za provjeru prosljeđivanja Adresa:</span><span class="sxs-lookup"><span data-stu-id="4e3d1-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="4e3d1-106">Odaberite **korisnike**  >  **aktivnih korisnika**.</span><span class="sxs-lookup"><span data-stu-id="4e3d1-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="4e3d1-107">Odaberite korisnika čiji je račun ugrožen.</span><span class="sxs-lookup"><span data-stu-id="4e3d1-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="4e3d1-108">U bočici koja će se prikazati proširite **postavke pošte**, a zatim kliknite **Uredi** za **Prosljeđivanje e-pošte**.</span><span class="sxs-lookup"><span data-stu-id="4e3d1-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="4e3d1-109">Uklonite sve adrese za prosljeđivanje koje ne prepoznajete.</span><span class="sxs-lookup"><span data-stu-id="4e3d1-109">Remove any forwarding addresses you don't recognize.</span></span>