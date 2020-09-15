---
title: Onemogućivanje vanjskih grupa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704120"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="14d9f-102">Onemogućivanje vanjskih grupa</span><span class="sxs-lookup"><span data-stu-id="14d9f-102">How to disable External Groups</span></span>

<span data-ttu-id="14d9f-103">Vanjska poruka servisa Yammer primjenjuje pravila prijenosa sustava Exchange (atrs), skup proaktivnih kontrola da bi se spriječilo zajedničko korištenje podataka o tvrtki.</span><span class="sxs-lookup"><span data-stu-id="14d9f-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="14d9f-104">Da biste korisnicima ograničili Stvaranje vanjskih grupa, morate konfigurirati pravilo prijenosa sustava Exchange (ETR), a zatim konfigurirati Yammer da koristi pravilo prijenosa sustava Exchange da bi blokirao vanjsku razmjenu poruka.</span><span class="sxs-lookup"><span data-stu-id="14d9f-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="14d9f-105">Kada stvorite pravilo u centru za administratore sustava Exchange Online, slijedite ove korake da biste postavili ETR za primjenu u servisu Yammer:</span><span class="sxs-lookup"><span data-stu-id="14d9f-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="14d9f-106">Prijavite se u Yammer kao ovjereni administrator, a zatim u **centru za administratore servisa Yammer**otvorite **Postavke C sadržaja i sigurnosne \> sigurnosti.**</span><span class="sxs-lookup"><span data-stu-id="14d9f-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="14d9f-107">U odjeljku **vanjsko razmjenu poruka**odaberite **Nametni pravila prijenosa sustava Exchange Online (atrs) u servisu Yammer.**</span><span class="sxs-lookup"><span data-stu-id="14d9f-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="14d9f-108">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="14d9f-108">Choose **Save**.</span></span>

<span data-ttu-id="14d9f-109">Dodatne informacije potražite u članku [onemogućivanje vanjskih poruka u mreži servisa Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="14d9f-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  