---
title: Izmjena Microsoftova ruba pomoću varijabli podatkovnog direktorija, a ne tvrdih puteva
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035013"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a><span data-ttu-id="91cf8-102">Izmjena Microsoftova ruba pomoću varijabli podatkovnog direktorija, a ne tvrdih puteva</span><span class="sxs-lookup"><span data-stu-id="91cf8-102">Modify Microsoft Edge by using data directory variables rather than hard-coded paths</span></span>

<span data-ttu-id="91cf8-103">Da biste, primjerice, u sustavu Windows pohranili podatke o profilu u odjeljku korisnika lokalnih aplikacija, a ne na zadanom mjestu, postavite pravilnik *Userdatadir* na **$ {local_app_data} \Edge\Profile**.</span><span class="sxs-lookup"><span data-stu-id="91cf8-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the *UserDataDir* policy to **${local_app_data}\Edge\Profile**.</span></span>

<span data-ttu-id="91cf8-104">Dodatne informacije potražite u članku [Stvaranje varijabli Microsoftovih podatkovnih direktorija](https://docs.microsoft.com/deployedge/microsoft-edge-policies)u pregledniku.</span><span class="sxs-lookup"><span data-stu-id="91cf8-104">For more information, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span></span>