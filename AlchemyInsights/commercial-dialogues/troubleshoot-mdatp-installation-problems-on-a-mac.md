---
title: Otklanjanje poteškoća s instalacijom MDATP-a na Macu
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743739"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="755a2-102">Otklanjanje poteškoća s instalacijom MDATP-a na Macu</span><span class="sxs-lookup"><span data-stu-id="755a2-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="755a2-103">Ako Ručna instalacija ne uspije, na stranici **sažetka** čarobnjaka za instalaciju prikazat će se sljedeća pogreška:</span><span class="sxs-lookup"><span data-stu-id="755a2-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="755a2-104">"Prilikom instalacije došlo je do pogreške.</span><span class="sxs-lookup"><span data-stu-id="755a2-104">"An error occurred during installation.</span></span> <span data-ttu-id="755a2-105">Instalacijski program naišao je na pogrešku koja je uzrokovala neuspjeh instalacije.</span><span class="sxs-lookup"><span data-stu-id="755a2-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="755a2-106">Zatražite pomoć od proizvođača softvera. "</span><span class="sxs-lookup"><span data-stu-id="755a2-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="755a2-107">Na stranici implementacije MDM-a stranica prikazuje i generički neuspjeh instalacije.</span><span class="sxs-lookup"><span data-stu-id="755a2-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="755a2-108">Iako ne prikazujemo točne pogreške krajnjim korisnicima, držimo datoteku zapisnika s napretkom instalacije u **/Library/logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="755a2-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="755a2-109">Svaka instalacija sesije dodaje se u ovu datoteku zapisnika.</span><span class="sxs-lookup"><span data-stu-id="755a2-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="755a2-110">Da biste mogli obaviti samo zadnju sesiju instalacije, koristite `sed` .</span><span class="sxs-lookup"><span data-stu-id="755a2-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="755a2-111">Dodatne informacije potražite u članku [Otklanjanje poteškoća s instalacijom za Microsoft Defender ATP za Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="755a2-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
