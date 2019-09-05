---
title: Kako onemogućiti vanjski grupe
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36739485"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="5292d-102">Kako onemogućiti vanjski grupe</span><span class="sxs-lookup"><span data-stu-id="5292d-102">How to disable External Groups</span></span>

<span data-ttu-id="5292d-103">Vanjski messaging primjenjuje Exchange prijevoza pravila (ETRs), postavite određene proaktivne kontrole da biste spriječili tvrtke informacije iz zajednički koristi za Yammer.</span><span class="sxs-lookup"><span data-stu-id="5292d-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="5292d-104">Za ograničavanje korisnicima stvaranje vanjskih grupa, potrebno je konfigurirati pravilo prijevoza Exchange (ETR), a zatim konfigurirajte Yammer koristiti pravilo Exchangeov Transport Blokiranje vanjskog messaging.</span><span class="sxs-lookup"><span data-stu-id="5292d-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="5292d-105">Kada ste stvorili pravilo u centru za Exchange Online admin, slijedite ove korake da biste postavili ETR za primjenu u servisu Yammer:</span><span class="sxs-lookup"><span data-stu-id="5292d-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="5292d-106">Prijavite se na Yammer kao administraciju provjereno i u **centru za administraciju servisa Yammer**, idite na C **sadržaja i sigurnosti \> sigurnosne postavke.**</span><span class="sxs-lookup"><span data-stu-id="5292d-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="5292d-107">U odjeljku **Vanjski Messaging**odaberite **nametnuti Exchange Online Exchange prijevoza pravila (ETRs) u servisu Yammer.**</span><span class="sxs-lookup"><span data-stu-id="5292d-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="5292d-108">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="5292d-108">Choose **Save**.</span></span>

<span data-ttu-id="5292d-109">Za dodatne informacije pogledajte [onemogućiti vanjski messaging u mrežu servisa Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="5292d-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  