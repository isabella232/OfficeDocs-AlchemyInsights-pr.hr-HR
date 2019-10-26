---
title: Kako onemogućiti vanjske grupe
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739485"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="d4c12-102">Kako onemogućiti vanjske grupe</span><span class="sxs-lookup"><span data-stu-id="d4c12-102">How to disable External Groups</span></span>

<span data-ttu-id="d4c12-103">Vanjska poruka tvrtke Yammer primjenjuje pravila razmjene sustava Exchange (ETRs), skup proaktivnih kontrola kako bi spriječio dijeljenje informacija o tvrtki.</span><span class="sxs-lookup"><span data-stu-id="d4c12-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="d4c12-104">Kako bi se korisnici ograničili od stvaranja vanjskih grupa, morate konfigurirati pravilo sustava Exchange (ETR), a zatim konfigurirati Yammer da koristi pravilo Exchange transport za blokiranje vanjskih poruka.</span><span class="sxs-lookup"><span data-stu-id="d4c12-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="d4c12-105">Nakon što kreirate pravilo u centru za administraciju sustava Exchange Online, slijedite ove korake da biste postavili ETR za primjenu u servisu Yammer:</span><span class="sxs-lookup"><span data-stu-id="d4c12-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="d4c12-106">Prijavite se na Yammer kao verificirani admin i u centru za **administraciju servisa Yammer**idite na C **sadržaj i sigurnosne \> sigurnosne postavke.**</span><span class="sxs-lookup"><span data-stu-id="d4c12-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="d4c12-107">U odjeljku **vanjske poruke**odaberite **Provedba pravila sustava Exchange Online Exchange (etrs) u servisu Yammer.**</span><span class="sxs-lookup"><span data-stu-id="d4c12-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="d4c12-108">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="d4c12-108">Choose **Save**.</span></span>

<span data-ttu-id="d4c12-109">Za više informacija pogledajte [Onemogući vanjsku razmjenu poruka u Yammer mreži](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="d4c12-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  