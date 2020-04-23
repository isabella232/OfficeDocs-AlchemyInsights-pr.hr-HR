---
title: Kako onemogućiti vanjske grupe
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720760"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="73398-102">Kako onemogućiti vanjske grupe</span><span class="sxs-lookup"><span data-stu-id="73398-102">How to disable External Groups</span></span>

<span data-ttu-id="73398-103">Vanjski mjesni poruka na servisu Yammer primjenjuje pravila prijenosa sustava Exchange (ETR), skup proaktivnih kontrola kako bi se spriječilo zajedničko korištenje informacija o poduzeću.</span><span class="sxs-lookup"><span data-stu-id="73398-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="73398-104">Da biste korisnicima ograničili stvaranje vanjskih grupa, morate konfigurirati pravilo prijenosa sustava Exchange (ETR), a zatim konfigurirati Yammer da koristi pravilo prijenosa sustava Exchange da bi blokirao vanjske poruke.</span><span class="sxs-lookup"><span data-stu-id="73398-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="73398-105">Nakon što stvorite pravilo u centru za administratore sustava Exchange Online, slijedite ove korake da biste postavili ETR za primjenu na servisu Yammer:</span><span class="sxs-lookup"><span data-stu-id="73398-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="73398-106">Prijavite se na Yammer kao provjereni administrator, a u centru za **administratore servisa Yammer**idite na C \*\*postavke sadržaja i sigurnosti. \> \*\*</span><span class="sxs-lookup"><span data-stu-id="73398-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="73398-107">U **odjeljku Vanjske poruke**odaberite **Nametni pravila prijenosa sustava Exchange (ETRs) na servisu Yammer.**</span><span class="sxs-lookup"><span data-stu-id="73398-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="73398-108">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="73398-108">Choose **Save**.</span></span>

<span data-ttu-id="73398-109">Dodatne informacije [potražite u odjeljku Onemogućivanje vanjskih poruka na mreži servisa Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="73398-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  