---
title: Ograničavanje sustava SharePoint Online na klasični način rada
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742461"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="98312-102">Ograničavanje sustava SharePoint Online na klasični način rada</span><span class="sxs-lookup"><span data-stu-id="98312-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="98312-103">Neke organizacije i dalje zahtijevaju doživljaj klasičnog načina rada.</span><span class="sxs-lookup"><span data-stu-id="98312-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="98312-104">Iako nema planova za uklanjanje klasičnog načina rada na granularnoj razini, više nije moguće ograničiti cijelu organizaciju (klijenta) na klasični način za popise i biblioteke.</span><span class="sxs-lookup"><span data-stu-id="98312-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="98312-105">Admin će imati sljedeće mogućnosti za upravljanje pojedinačnim popisima i bibliotekama u klasičnom načinu rada pomoću granularnih prekidača za isključivanje koje pružamo na sljedećim razinama:</span><span class="sxs-lookup"><span data-stu-id="98312-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="98312-106">zbirka web-mjesta</span><span class="sxs-lookup"><span data-stu-id="98312-106">site collection</span></span>
- <span data-ttu-id="98312-107">Stranice</span><span class="sxs-lookup"><span data-stu-id="98312-107">site</span></span>
- <span data-ttu-id="98312-108">Popis</span><span class="sxs-lookup"><span data-stu-id="98312-108">list</span></span>
- <span data-ttu-id="98312-109">Biblioteka</span><span class="sxs-lookup"><span data-stu-id="98312-109">library</span></span>

<span data-ttu-id="98312-110">Osim toga, popisi koji koriste određene značajke i prilagodbe koje moderni ne podržavaju i dalje će se automatski prebaciti u klasični način rada.</span><span class="sxs-lookup"><span data-stu-id="98312-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="98312-111">Početkom travnja 1, 2019, proces onemogućiti razinu stanara isključiti iz modernog popisa i knjižnice će početi i nastaviti do svibnja 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="98312-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="98312-112">Popisi i biblioteke koji su u klasičnom načinu rada kao rezultat isključivanja klijenta automatski će se prebaciti na moderno.</span><span class="sxs-lookup"><span data-stu-id="98312-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="98312-113">Ako vam je potreban klasični način pogledajte više informacija [ovdje](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) i PnP Powershell upute [ovdje](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) koji opisuje opcije i alate koje možete koristiti danas za korištenje klasičnog načina rada iskustvo.</span><span class="sxs-lookup"><span data-stu-id="98312-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
