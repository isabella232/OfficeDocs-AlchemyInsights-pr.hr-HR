---
title: Automatsko šifriranje poruka e-pošte sustava Office 365 poslane na određene domene
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743685"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="a1b90-102">Automatsko šifriranje poruka e-pošte sustava Office 365 poslane na određene domene</span><span class="sxs-lookup"><span data-stu-id="a1b90-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="a1b90-103">U [centru za administratore sustava Exchange](https://outlook.office365.com/ecp/)odaberite **tijek pošte > pravila**.</span><span class="sxs-lookup"><span data-stu-id="a1b90-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="a1b90-104">Kliknite ikonu **Novo (+)** , a zatim kliknite **Primijeni šifriranje poruka i zaštita prava u sustavu Office 365 na poruke**.</span><span class="sxs-lookup"><span data-stu-id="a1b90-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="a1b90-105">U **naziv** unesite naziv pravila, primjerice *Šifriraj poruke poslane u contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="a1b90-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="a1b90-106">U odjeljku **Primijeni ovo pravilo** odaberite **Primatelj > domena**.</span><span class="sxs-lookup"><span data-stu-id="a1b90-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="a1b90-107">Unesite naziv domene, primjerice **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="a1b90-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="a1b90-108">Kliknite ikonu **Dodaj (+)** , a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="a1b90-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="a1b90-109">Pokraj polja **učinite sljedeće** kliknite **Odaberi jednu**.</span><span class="sxs-lookup"><span data-stu-id="a1b90-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="a1b90-110">Na padajućem izborniku **predloška RMS** -a odaberite **Šifriraj**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="a1b90-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="a1b90-111">(Ako ne vidite tu mogućnost, to znači da vaš plan ne obuhvaća automatsko šifriranje.</span><span class="sxs-lookup"><span data-stu-id="a1b90-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="a1b90-112">No, možete ga dodati!)</span><span class="sxs-lookup"><span data-stu-id="a1b90-112">But you can add it!)</span></span>
9. <span data-ttu-id="a1b90-113">Odaberite bilo koji neobavezni odabir (s popisa neobaveznih odabira koje možete učiniti u ovom trenutku, od kojih se mnogi mogu vratiti uz zadanu postavku za jednostavnost).</span><span class="sxs-lookup"><span data-stu-id="a1b90-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="a1b90-114">Kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="a1b90-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a1b90-115">Uvijek se možete vratiti i urediti to pravilo kasnije.</span><span class="sxs-lookup"><span data-stu-id="a1b90-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="a1b90-116">Dodatne informacije o stvaranju pravila šifriranja potražite [u članku definiranje pravila tijeka pošte za šifriranje poruka e-pošte u sustavu Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="a1b90-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>