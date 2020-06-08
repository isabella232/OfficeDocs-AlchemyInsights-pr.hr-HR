---
title: Omogućivanje otvaranja naslijeđenih dijaloga ugradnjom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: ca0894849e95fd69acd2065c3f065547231a07f9
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204652"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="fb5df-102">Omogućivanje otvaranja naslijeđenih dijaloga ugradnjom</span><span class="sxs-lookup"><span data-stu-id="fb5df-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="fb5df-103">**Simptom**</span><span class="sxs-lookup"><span data-stu-id="fb5df-103">**Symptom**</span></span>

<span data-ttu-id="fb5df-104">Korisnici ne mogu otvoriti izvješća.</span><span class="sxs-lookup"><span data-stu-id="fb5df-104">Users are unable to open reports.</span></span> <span data-ttu-id="fb5df-105">"Nešto je pošlo po zlu.</span><span class="sxs-lookup"><span data-stu-id="fb5df-105">"Something has gone wrong.</span></span> <span data-ttu-id="fb5df-106">Provjerite tehničke detalje za više detalja."</span><span class="sxs-lookup"><span data-stu-id="fb5df-106">Check technical details for more details."</span></span>

<span data-ttu-id="fb5df-107">**Uzrokovati**</span><span class="sxs-lookup"><span data-stu-id="fb5df-107">**Cause**</span></span>

<span data-ttu-id="fb5df-108">Izvješća se ne učitavaju u UCI s pogreškom "Opisnik obrasca je null ili nije definiran."</span><span class="sxs-lookup"><span data-stu-id="fb5df-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="fb5df-109">Izvješća u UCI-ju i dalje zahtijevaju naslijeđene dijaloge, tako da klijentov sustav mora omogućiti omogućeno *nasljeđivanje dijagnoze.*</span><span class="sxs-lookup"><span data-stu-id="fb5df-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="fb5df-110">**Rješenje**</span><span class="sxs-lookup"><span data-stu-id="fb5df-110">**Solution**</span></span>

1. <span data-ttu-id="fb5df-111">Idite na **karticu Postavke >administracije > postavke sustava > Općenito**.</span><span class="sxs-lookup"><span data-stu-id="fb5df-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="fb5df-112">Postavite "Omogući ugrađivanje određenih naslijeđenih dijaloga u klijentu preglednika objedinjenog sučelja" na **Da**.</span><span class="sxs-lookup"><span data-stu-id="fb5df-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
