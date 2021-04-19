---
title: Omogućivanje ugrađivanja naslijeđenih dijaloških okvira radi otvaranja izvješća
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814256"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="207f2-102">Omogućivanje ugrađivanja naslijeđenih dijaloških okvira radi otvaranja izvješća</span><span class="sxs-lookup"><span data-stu-id="207f2-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="207f2-103">**Simptom**</span><span class="sxs-lookup"><span data-stu-id="207f2-103">**Symptom**</span></span>

<span data-ttu-id="207f2-104">Korisnici ne mogu otvarati izvješća.</span><span class="sxs-lookup"><span data-stu-id="207f2-104">Users are unable to open reports.</span></span> <span data-ttu-id="207f2-105">"Nešto nije u redu.</span><span class="sxs-lookup"><span data-stu-id="207f2-105">"Something has gone wrong.</span></span> <span data-ttu-id="207f2-106">Dodatne pojedinosti potražite u tehničkim pojedinostima."</span><span class="sxs-lookup"><span data-stu-id="207f2-106">Check technical details for more details."</span></span>

<span data-ttu-id="207f2-107">**Uzrok**</span><span class="sxs-lookup"><span data-stu-id="207f2-107">**Cause**</span></span>

<span data-ttu-id="207f2-108">Izvješća se ne mogu učitati u UCI uz pogrešku "Opisnik obrasca ima vrijednost null ili nije definirana".</span><span class="sxs-lookup"><span data-stu-id="207f2-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="207f2-109">Izvješća u UCI-jem i dalje zahtijevaju naslijeđene dijaloški okvire, pa klijentov sustav mora *omogućiti omogućivo* omogućivo stvaranje sustava.</span><span class="sxs-lookup"><span data-stu-id="207f2-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="207f2-110">**Rješenje**</span><span class="sxs-lookup"><span data-stu-id="207f2-110">**Solution**</span></span>

1. <span data-ttu-id="207f2-111">Otvorite **Postavke >Administracija > postavke sustava > općenito**.</span><span class="sxs-lookup"><span data-stu-id="207f2-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="207f2-112">Postavite "Enable embedding of certain legacy dialogs in Unified Interface browser client" (Omogući ugrađivanje određenih naslijeđenih dijaloških okvira u klijentu preglednika sjedinjenog sučelja) na **Da**.</span><span class="sxs-lookup"><span data-stu-id="207f2-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
