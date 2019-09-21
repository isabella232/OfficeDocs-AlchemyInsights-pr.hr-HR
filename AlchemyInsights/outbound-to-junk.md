---
title: Izlazna e-pošta u mapu bezvrijedne e-pošte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 371d2c46e9048365fd343145330536bd9cf1db82
ms.sourcegitcommit: 1002f510fadb92c143cd6bbb60b42a851d5a38e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/20/2019
ms.locfileid: "37062748"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="198a4-102">Izlazna e-pošta u mapu bezvrijedne e-pošte</span><span class="sxs-lookup"><span data-stu-id="198a4-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="198a4-103">Ako ste vidjeli izlazne poruke označene kao junk, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="198a4-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="198a4-104">Ako već niste, razmotrite [Konfiguriranje obavijesti o izlaznim spam pravilima](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="198a4-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="198a4-105">Koristite [trag poruke](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) da biste vidjeli ima li izlazna poruka **neželjenu** vrijednost događaja uz dodatni detalj: **koristite bazen visokog rizika za isporuku**.</span><span class="sxs-lookup"><span data-stu-id="198a4-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="198a4-106">Za ove poruke provjerite sadržaj poruke da biste vidjeli što se može smatrati spam.</span><span class="sxs-lookup"><span data-stu-id="198a4-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="198a4-107">Na primjer, potpisi ponekad mogu uzrokovati probleme za mnoge korisnike.</span><span class="sxs-lookup"><span data-stu-id="198a4-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="198a4-108">Ako imate više primjera zakonitih izlaznih poruka koje su označene kao junk, otvorite ulaznicu za podršku i zatražite od agenta za podršku da vaše poruke šalju kao lažne pozitivne na naše neželjene analitičare.</span><span class="sxs-lookup"><span data-stu-id="198a4-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="198a4-109">Budite spremni pružiti ogledne poruke koje uključuju sva zaglavlja poruka.</span><span class="sxs-lookup"><span data-stu-id="198a4-109">Be prepared to provide sample messages that include all message headers.</span></span>
