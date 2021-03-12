---
title: Konfiguriranje i provjera autentičnosti izuzeća za MDATP na računalu s Linuxom
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
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743681"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="1fa41-102">Konfiguriranje i provjera autentičnosti izuzeća za MDATP na računalu s Linuxom</span><span class="sxs-lookup"><span data-stu-id="1fa41-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="1fa41-103">Moguće je isključiti određene datoteke, mape, procese te datoteke koje se otvaraju procesom iz MDATP skeniranja.</span><span class="sxs-lookup"><span data-stu-id="1fa41-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="1fa41-104">Isključenja pomažu u sprječavanju neispravnog otkrivanja softvera i datoteka koje su jedinstvene ili prilagođene vašoj tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="1fa41-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="1fa41-105">Isključenja također pomažu ublažiti poteškoće s performansama uzrokovane MDATP-om.</span><span class="sxs-lookup"><span data-stu-id="1fa41-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="1fa41-106">Dodatne informacije potražite u članku [Konfiguriranje i provjera autentičnosti isključenja za MDATP za Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="1fa41-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1fa41-107">Isključenja opisana u ovom članku ne primjenjuju se na druge mogućnosti MDATP za Linux, uključujući krajnje točke otkrivanja i odaziva (EDR).</span><span class="sxs-lookup"><span data-stu-id="1fa41-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="1fa41-108">Datoteke koje izostavite pomoću metoda opisanih u ovom članku i dalje mogu pokrenuti obavijesti o EDR-u i druge mogućnosti otkrivanja.</span><span class="sxs-lookup"><span data-stu-id="1fa41-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
