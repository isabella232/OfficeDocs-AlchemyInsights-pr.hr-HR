---
title: Automatski Šifriraj određene poruke e-pošte iz sustava Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523562"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="9aadf-102">Automatski Šifriraj određene poruke e-pošte iz sustava Office 365</span><span class="sxs-lookup"><span data-stu-id="9aadf-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="9aadf-103">U [centru za administratore sustava Exchange](https://outlook.office365.com/ecp/)odaberite **tijek pošte > pravila**.</span><span class="sxs-lookup"><span data-stu-id="9aadf-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="9aadf-104">Kliknite ikonu **Novo (+)** , a zatim kliknite **Primijeni šifriranje poruka i zaštita prava u sustavu Office 365 na poruke**.</span><span class="sxs-lookup"><span data-stu-id="9aadf-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="9aadf-105">U **naziv** unesite naziv pravila, primjerice *Šifriraj sve poruke*.</span><span class="sxs-lookup"><span data-stu-id="9aadf-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="9aadf-106">U odjeljku **Primijeni ovo pravilo** odaberite **[Primijeni na sve poruke]**.</span><span class="sxs-lookup"><span data-stu-id="9aadf-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="9aadf-107">Pokraj polja **učinite sljedeće** kliknite **Odaberi jednu**.</span><span class="sxs-lookup"><span data-stu-id="9aadf-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="9aadf-108">Na padajućem izborniku **predloška RMS** -a odaberite **Šifriraj**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="9aadf-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="9aadf-109">(Ako ne vidite tu mogućnost, to znači da vaš plan ne obuhvaća automatsko šifriranje.</span><span class="sxs-lookup"><span data-stu-id="9aadf-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="9aadf-110">No, možete ga dodati!)</span><span class="sxs-lookup"><span data-stu-id="9aadf-110">But you can add it!)</span></span>
7. <span data-ttu-id="9aadf-111">Potvrdite okvir **nadziranje ovog pravila s razinom težine** , a zatim odaberite željenu razinu.</span><span class="sxs-lookup"><span data-stu-id="9aadf-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="9aadf-112">Ako vaša tvrtka ima ugovorne obveze za sve šifrirane poruke e-pošte, preporučujem Postavljanje razine na **visoku**.</span><span class="sxs-lookup"><span data-stu-id="9aadf-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="9aadf-113">U odjeljku **Odaberite model za ovo pravilo** kliknite **Nametni**.</span><span class="sxs-lookup"><span data-stu-id="9aadf-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="9aadf-114">Odaberite bilo koji neobavezni odabir (s popisa neobaveznih odabira koje možete učiniti u ovom trenutku, od kojih se mnogi mogu vratiti uz zadanu postavku za jednostavnost).</span><span class="sxs-lookup"><span data-stu-id="9aadf-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="9aadf-115">Kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="9aadf-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9aadf-116">Uvijek se možete vratiti i urediti to pravilo kasnije.</span><span class="sxs-lookup"><span data-stu-id="9aadf-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="9aadf-117">Dodatne informacije o stvaranju pravila šifriranja potražite [u članku definiranje pravila tijeka pošte za šifriranje poruka e-pošte u sustavu Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="9aadf-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

