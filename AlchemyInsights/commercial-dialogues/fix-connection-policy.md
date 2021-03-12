---
title: Rješavanje pravilnika o povezivanju
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743867"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="bd9fd-102">Rješavanje pravilnika o povezivanju</span><span class="sxs-lookup"><span data-stu-id="bd9fd-102">Fix connection policy</span></span>

<span data-ttu-id="bd9fd-103">Poruka e-pošte označena je sigurnim i isporučena u korisničku ulaznu poštu jer je IP adresa slanja označena kao sigurna u pravilima filtra veze.</span><span class="sxs-lookup"><span data-stu-id="bd9fd-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="bd9fd-104">Da biste pregledali pravilnik, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="bd9fd-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="bd9fd-105">Idite na [centar za sigurnost & sustava Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), a zatim otvorite pravilo za **Upravljanje prijetnjama** za  >    >  [zaštitu od neželjene pošte](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="bd9fd-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="bd9fd-106">Na kartici **Prilagođena** odaberite **pravilnik o filtriranju veze**, a zatim odaberite **Uređivanje pravilnika**.</span><span class="sxs-lookup"><span data-stu-id="bd9fd-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="bd9fd-107">Pregledajte popis **dozvola za IP** .</span><span class="sxs-lookup"><span data-stu-id="bd9fd-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="bd9fd-108">Pogledajte je li omogućen **popis sigurnih popisa** .</span><span class="sxs-lookup"><span data-stu-id="bd9fd-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="bd9fd-109">Microsoftovi pretplatnici na izvore drugih davatelja pouzdanih pošiljatelja.</span><span class="sxs-lookup"><span data-stu-id="bd9fd-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="bd9fd-110">Ako je omogućen **popis sigurnog popisa** , ti pouzdani pošiljatelji nisu pogrešno označeni kao neželjena pošta.</span><span class="sxs-lookup"><span data-stu-id="bd9fd-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="bd9fd-111">Preporučujem vam da odaberete tu mogućnost, jer će to smanjiti broj FALSE pozitivnih (dobra pošta koja je klasificirana kao spam) koju primate.</span><span class="sxs-lookup"><span data-stu-id="bd9fd-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
