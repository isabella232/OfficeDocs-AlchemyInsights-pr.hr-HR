---
title: Izlazna e-pošta u mapu Bezvrijedna e-pošta
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769175"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="2f516-102">Izlazna e-pošta u mapu Bezvrijedna e-pošta</span><span class="sxs-lookup"><span data-stu-id="2f516-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="2f516-103">Ako se odlazne poruke označavaju kao bezvrijedne, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="2f516-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="2f516-104">Ako to već niste učinili, razmotrite [Konfiguriranje obavijesti o pravilima izlazne neželjene pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="2f516-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="2f516-105">Koristite [Praćenje poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) da biste vidjeli ako izlazna poruka sadrži **neželjenu** vrijednost događaja uz dodatni detalj: **korištenje bazena visokog rizika**.</span><span class="sxs-lookup"><span data-stu-id="2f516-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="2f516-106">Za ove poruke provjerite sadržaj poruke da biste vidjeli što se može smatrati neželjenom poštom.</span><span class="sxs-lookup"><span data-stu-id="2f516-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="2f516-107">Potpisi, primjerice, ponekad mogu prouzročiti probleme za mnoge korisnike.</span><span class="sxs-lookup"><span data-stu-id="2f516-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="2f516-108">Ako imate više primjera legitimnih izlaznog poruka koje su označene kao bezvrijedne, otvorite karticu za podršku i zatražite od agenta za podršku da poruke pošalju kao lažne rezultate našim analitičarima neželjene pošte.</span><span class="sxs-lookup"><span data-stu-id="2f516-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="2f516-109">Budite spremni pružiti ogledne poruke koje obuhvaćaju sva zaglavlja poruka.</span><span class="sxs-lookup"><span data-stu-id="2f516-109">Be prepared to provide sample messages that include all message headers.</span></span>
