---
title: Rješavanje pravilnika o klijentu (prijelaz na akciju)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692799"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="9f485-102">Rješavanje pravilnika o klijentu (prijelaz na akciju)</span><span class="sxs-lookup"><span data-stu-id="9f485-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="9f485-103">Pravilnik o suzbijanju neželjene pošte u vašem zakupcu utjecao je na ovu poruku.</span><span class="sxs-lookup"><span data-stu-id="9f485-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="9f485-104">Da biste pregledali pravilnik, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="9f485-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="9f485-105">Idite na [centar za sigurnost & sustava Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), a zatim otvorite pravilo za **Upravljanje prijetnjama** za  >    >  [zaštitu od neželjene pošte](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="9f485-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="9f485-106">Provjerite prikazuje li **izvor pravilnika** sljedeće:  **Dodavanje-XHeader/Modifysubject/preusmjeravanje/Izbriši/bez akcije/Skrivena kopija poruka**</span><span class="sxs-lookup"><span data-stu-id="9f485-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="9f485-107">Ako je tako, na kartici **Prilagođeno** provjerite postavke Pravilnika koja je utjecala na poruku.</span><span class="sxs-lookup"><span data-stu-id="9f485-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="9f485-108">Moguće je da su **standardne postavke** primijenjene na sve klijente zaštite servisa Exchange Online utjecali na poruku.</span><span class="sxs-lookup"><span data-stu-id="9f485-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="9f485-109">Dodatne informacije o konfiguriranju pravilnika filtra za neželjenu poštu potražite u članku [Konfiguriranje pravilnika filtra za neželjenu poštu](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="9f485-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
