---
title: Ograniči SharePoint Online klasični način
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761751"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="0c640-102">Ograniči SharePoint Online klasični način</span><span class="sxs-lookup"><span data-stu-id="0c640-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="0c640-103">Neke organizacije i dalje zahtijevaju klasični način doživljaj.</span><span class="sxs-lookup"><span data-stu-id="0c640-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="0c640-104">Dok postoje planovi za uklanjanje klasični način zrnaste razini, više nije moguće ograničiti cijelu organizaciju (klijentske) klasični način za popise i biblioteke.</span><span class="sxs-lookup"><span data-stu-id="0c640-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="0c640-105">Administrator će imati sljedeće mogućnosti za upravljanje pojedinačnim popisima i bibliotekama u klasični način korištenja zrnaste opt-out popis parametara koje pružamo sljedeće razine:</span><span class="sxs-lookup"><span data-stu-id="0c640-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="0c640-106">Zbirka web-mjesta</span><span class="sxs-lookup"><span data-stu-id="0c640-106">site collection</span></span>
- <span data-ttu-id="0c640-107">web-mjesta</span><span class="sxs-lookup"><span data-stu-id="0c640-107">site</span></span>
- <span data-ttu-id="0c640-108">Popis</span><span class="sxs-lookup"><span data-stu-id="0c640-108">list</span></span>
- <span data-ttu-id="0c640-109">Biblioteka</span><span class="sxs-lookup"><span data-stu-id="0c640-109">library</span></span>

<span data-ttu-id="0c640-110">Osim toga, popisi koji koristite određene značajke i prilagodbe koje ne podržava Moderni će i dalje biti automatski prebacio na klasični način.</span><span class="sxs-lookup"><span data-stu-id="0c640-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="0c640-111">Početak Travanj 1, 2019, postupka onemogućili razinu klijentske budućih Moderna popisa i biblioteke će pokrenuti i nastavite kroz možda 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="0c640-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="0c640-112">Popisi i biblioteke koji su u klasični način zbog klijentske opt-out popis automatski biti pomaknute za Moderna.</span><span class="sxs-lookup"><span data-stu-id="0c640-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="0c640-113">Ako zahtijevaju klasični način pogledajte dodatne informacije [ovdje](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) i uputa PnP Powershell [ovdje](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) koji opisuje mogućnosti i alate možete koristiti danas koristi klasični način doživljaj.</span><span class="sxs-lookup"><span data-stu-id="0c640-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
