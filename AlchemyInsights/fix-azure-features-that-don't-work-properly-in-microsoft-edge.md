---
title: Što učiniti ako značajke Azure ne funkcioniraju pravilno u pregledniku Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583227"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="6f2c1-102">Što učiniti ako značajke Azure ne funkcioniraju pravilno u pregledniku Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="6f2c1-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="6f2c1-103">Microsoft Edge sadrži [poznate probleme](https://go.microsoft.com/fwlink/?linkid=2140608) koji se odnose na sigurnosne zone i mogu utjecati na to kako se korisnici Azure prijave u centar za administratore sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="6f2c1-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="6f2c1-104">Ako imate problema s upotrebom značajki Azure s programom Microsoft Edge, isprobajte sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="6f2c1-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="6f2c1-105">Na izborniku **Start** potražite **mogućnosti interneta** i odaberite ga.</span><span class="sxs-lookup"><span data-stu-id="6f2c1-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="6f2c1-106">U dijaloškom okviru **internetska svojstva** otvorite karticu **Sigurnost** .</span><span class="sxs-lookup"><span data-stu-id="6f2c1-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="6f2c1-107">Odaberite zonu **pouzdanih web-mjesta** , a zatim odaberite gumb **web-mjesta** .</span><span class="sxs-lookup"><span data-stu-id="6f2c1-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="6f2c1-108">U dijaloškom okviru **pouzdana web-mjesta** Dodajte URL pristupnika, kao [https://login.microsoftonline.com](https://login.microsoftonline.com) i [https://login.live.com](https://login.live.com) , a zatim odaberite **Zatvori**.</span><span class="sxs-lookup"><span data-stu-id="6f2c1-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="6f2c1-109">U dijaloškom okviru **internetska svojstva** otvorite karticu **Zaštita privatnosti** .</span><span class="sxs-lookup"><span data-stu-id="6f2c1-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="6f2c1-110">U odjeljku **blokator skočnih prozora** odaberite **Postavke**.</span><span class="sxs-lookup"><span data-stu-id="6f2c1-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="6f2c1-111">U dijaloškom okviru koji će se otvoriti Dodajte URL pristupnika, kao [https://login.microsoftonline.com](https://login.microsoftonline.com) i [https://login.live.com](https://login.live.com) , a zatim odaberite **Zatvori**.</span><span class="sxs-lookup"><span data-stu-id="6f2c1-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
