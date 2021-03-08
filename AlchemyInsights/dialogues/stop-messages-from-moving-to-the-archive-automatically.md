---
title: Automatsko zaustavljanje poruka od preseljenja u arhivu
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524102"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="ad934-102">Automatsko zaustavljanje poruka od preseljenja u arhivu</span><span class="sxs-lookup"><span data-stu-id="ad934-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="ad934-103">Ako koristite pravilnik o zadržavanju, možete promijeniti starost zadržavanja u tom pravilniku radi automatskog zaustavljanja poruka arhiviranja.</span><span class="sxs-lookup"><span data-stu-id="ad934-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="ad934-104">Evo i kako:</span><span class="sxs-lookup"><span data-stu-id="ad934-104">Here's how:</span></span>

1. <span data-ttu-id="ad934-105">U [centru za administratore sustava Exchange](https://go.microsoft.com/fwlink/?linkid=2059104)odaberite oznake zadržavanja za **Upravljanje usklađivanjem**  >  .</span><span class="sxs-lookup"><span data-stu-id="ad934-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="ad934-106">Pronađite svoj premještanje da biste arhivirali oznaku zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="ad934-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="ad934-107">U oznake zadržavanja promijenite razdoblje zadržavanja (razdoblje arhiviranja) da **nikada ne** biste zaustavili automatsko arhiviranje stavki pomoću pravilnika o zadržavanju.</span><span class="sxs-lookup"><span data-stu-id="ad934-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="ad934-108">Time ćete promijeniti postavku arhiviranja za sve poštanske sandučiće s tom oznakom zadržavanja koja se primjenjuje na njih.</span><span class="sxs-lookup"><span data-stu-id="ad934-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
