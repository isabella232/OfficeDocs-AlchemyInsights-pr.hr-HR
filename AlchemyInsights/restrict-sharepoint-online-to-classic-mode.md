---
title: Ograniči SharePoint online na klasični način rada
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048752"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="294fb-102">Ograniči SharePoint online na klasični način rada</span><span class="sxs-lookup"><span data-stu-id="294fb-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="294fb-103">Neke organizacije još uvijek zahtijevaju klasično iskustvo načina rada.</span><span class="sxs-lookup"><span data-stu-id="294fb-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="294fb-104">Iako nema planova za uklanjanje klasičnog načina rada na granularnoj razini, više nije moguće ograničiti cijelu organizaciju (stanar) na klasični način za popise i biblioteke.</span><span class="sxs-lookup"><span data-stu-id="294fb-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="294fb-105">Admin će imati sljedeće mogućnosti za upravljanje pojedinačnim popisima i bibliotekama u klasičnom načinu rada pomoću granularnih isključivanja prekidača koje pružamo na sljedećim razinama:</span><span class="sxs-lookup"><span data-stu-id="294fb-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="294fb-106">Zbirka web-mjesta</span><span class="sxs-lookup"><span data-stu-id="294fb-106">site collection</span></span>
- <span data-ttu-id="294fb-107">Stranice</span><span class="sxs-lookup"><span data-stu-id="294fb-107">site</span></span>
- <span data-ttu-id="294fb-108">Popis</span><span class="sxs-lookup"><span data-stu-id="294fb-108">list</span></span>
- <span data-ttu-id="294fb-109">Biblioteka</span><span class="sxs-lookup"><span data-stu-id="294fb-109">library</span></span>

<span data-ttu-id="294fb-110">Osim toga, popisi koji koriste određene značajke i prilagodbe koje ne podržavaju moderni i dalje će se automatski prebaciti u klasični način rada.</span><span class="sxs-lookup"><span data-stu-id="294fb-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="294fb-111">Počevši Travanj 1, 2019, proces onemogućiti klijentsku razinu isključiti od modernog popisa i knjižnice će početi i nastaviti kroz Svibanj 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="294fb-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="294fb-112">Popisi i biblioteke koje su u klasičnom načinu rada kao rezultat isključivanja stanara automatski će se prebaciti na moderni.</span><span class="sxs-lookup"><span data-stu-id="294fb-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="294fb-113">Ako vam je potreban klasični način Pogledajte više informacija [ovdje](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) i PNP PowerShell instrukcije [ovdje](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) koji opisuje opcije i alate koje možete koristiti danas za korištenje klasični način iskustva.</span><span class="sxs-lookup"><span data-stu-id="294fb-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
