---
title: Izlazna e-pošta u mapu Bezvrijedna e-pošta
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 2350586e95f316061ff855d152e86db0547eb209
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761160"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="2c49f-102">Izlazna e-pošta u mapu Bezvrijedna e-pošta</span><span class="sxs-lookup"><span data-stu-id="2c49f-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="2c49f-103">Ako vam se izlazne poruke označavaju kao Bezvrijedno, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="2c49f-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="2c49f-104">Ako to već niste učinili, razmislite o [konfiguriranju obavijesti o odlaznim spam pravilima](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="2c49f-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="2c49f-105">Upotrijebite [praćenje poruka](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) da biste vidjeli ima li izlazna poruka vrijednost događaja **Neželjena pošta** s dodatnim pojedinostima: **Koristite skup za isporuku visokog rizika**.</span><span class="sxs-lookup"><span data-stu-id="2c49f-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="2c49f-106">Za te poruke provjerite sadržaj poruke da biste vidjeli što se može smatrati neželjenom poštom.</span><span class="sxs-lookup"><span data-stu-id="2c49f-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="2c49f-107">Na primjer, potpisi ponekad mogu uzrokovati probleme za mnoge korisnike.</span><span class="sxs-lookup"><span data-stu-id="2c49f-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="2c49f-108">Ako imate više primjera legitimnih izlaznih poruka koje se označavaju kao Bezvrijedno, otvorite ulaznicu za podršku i zamolite agenta za podršku da pošalje vaše poruke kao lažno pozitivne poruke našim analitičarima neželjene pošte.</span><span class="sxs-lookup"><span data-stu-id="2c49f-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="2c49f-109">Budite spremni pružiti ogledne poruke koje uključuju sva zaglavlja poruka.</span><span class="sxs-lookup"><span data-stu-id="2c49f-109">Be prepared to provide sample messages that include all message headers.</span></span>
