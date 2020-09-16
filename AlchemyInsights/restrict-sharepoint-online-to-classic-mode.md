---
title: Ograničavanje sustava SharePoint online na klasičan način rada
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751414"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="149c0-102">Ograničavanje sustava SharePoint online na klasičan način rada</span><span class="sxs-lookup"><span data-stu-id="149c0-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="149c0-103">Neke ustanove i dalje zahtijevaju klasično iskustvo načina rada.</span><span class="sxs-lookup"><span data-stu-id="149c0-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="149c0-104">Iako nema planova za uklanjanje klasičnog načina rada na granulacijskom nivou, više nije moguće ograničiti cijelu organizaciju (korisnika) na klasični način za popise i biblioteke.</span><span class="sxs-lookup"><span data-stu-id="149c0-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="149c0-105">Administrator će imati sljedeće mogućnosti za upravljanje pojedinačnim popisima i bibliotekama u klasičnom načinu rada uz Granularne parametre isključivanja koje dajemo na sljedećim razinama:</span><span class="sxs-lookup"><span data-stu-id="149c0-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="149c0-106">Zbirka web-mjesta</span><span class="sxs-lookup"><span data-stu-id="149c0-106">site collection</span></span>
- <span data-ttu-id="149c0-107">stranice</span><span class="sxs-lookup"><span data-stu-id="149c0-107">site</span></span>
- <span data-ttu-id="149c0-108">popis</span><span class="sxs-lookup"><span data-stu-id="149c0-108">list</span></span>
- <span data-ttu-id="149c0-109">biblioteka</span><span class="sxs-lookup"><span data-stu-id="149c0-109">library</span></span>

<span data-ttu-id="149c0-110">Osim toga, popisi koji koriste određene značajke i prilagodbe koje moderni neće podržavati i dalje će se automatski prebaciti u klasični način rada.</span><span class="sxs-lookup"><span data-stu-id="149c0-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="149c0-111">Počevši od travnja 1, 2019, postupak za onemogućivanje izuzeća iz modernog popisa i biblioteka započet će i nastavit će se kroz Svibanj 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="149c0-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="149c0-112">Popisi i biblioteke koji su u klasičnom načinu rada kao rezultat izuzećih korisnika automatski će se pomaknuti na moderno.</span><span class="sxs-lookup"><span data-stu-id="149c0-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="149c0-113">Ako vam je potreban klasičan način rada, Pogledajte dodatne informacije [ovdje](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) i upute za PNP PowerShell [ovdje](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) koje opisuju mogućnosti i alate koje danas možete koristiti da biste koristili klasičan način rada.</span><span class="sxs-lookup"><span data-stu-id="149c0-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
