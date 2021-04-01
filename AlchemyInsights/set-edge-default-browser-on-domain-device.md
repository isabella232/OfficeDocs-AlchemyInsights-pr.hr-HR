---
title: Postavljanje preglednika Microsoft Edge kao zadanog preglednika na uređaju pridruženom domeni
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491371"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="d36dc-102">Postavljanje preglednika Microsoft Edge kao zadanog preglednika na uređaju pridruženom domeni</span><span class="sxs-lookup"><span data-stu-id="d36dc-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="d36dc-103">Postavite Microsoft Edge kao zadani preglednik:</span><span class="sxs-lookup"><span data-stu-id="d36dc-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="d36dc-104">[Stvorite zadanu konfiguracijsku datoteku pridruživanja](https://go.microsoft.com/fwlink/?linkid=2132437) i pohranite je lokalno ili na mrežno zajedničko korištenje.</span><span class="sxs-lookup"><span data-stu-id="d36dc-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="d36dc-105">Otvorite uređivač pravilnika grupe, a zatim otvorite Administratorski predlošci  >  **konfiguracije računala**  >  **Eksplorer za datoteke**  >  **komponenti sustava** Windows .</span><span class="sxs-lookup"><span data-stu-id="d36dc-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="d36dc-106">Odaberite **Postavi zadanu konfiguracijsku datoteku pridruživanja**.</span><span class="sxs-lookup"><span data-stu-id="d36dc-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="d36dc-107">Odaberite **Postavka pravilnika**, a zatim **Omogućeno**.</span><span class="sxs-lookup"><span data-stu-id="d36dc-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="d36dc-108">U **odjeljku** Mogućnosti unesite mjesto zadane konfiguracijske datoteke pridruživanja, a zatim odaberite U **redu**.</span><span class="sxs-lookup"><span data-stu-id="d36dc-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
