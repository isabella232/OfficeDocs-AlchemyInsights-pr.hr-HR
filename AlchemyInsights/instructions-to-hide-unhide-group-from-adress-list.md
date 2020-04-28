---
title: Upute za skrivanje/otkrivanje grupe s popisa adresa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908336"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="704c2-102">Skrivanje grupe za Microsoft 365 s popisa adresa (GAL)</span><span class="sxs-lookup"><span data-stu-id="704c2-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="704c2-103">Da biste sakrili grupu sustava Microsoft 365 s popisa adresa (GAL) klijenata sustava Exchange (kao što su Outlook ili OWA), koristite sljedeću naredbu u EXO ljuski:</span><span class="sxs-lookup"><span data-stu-id="704c2-103">To hide an Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="704c2-104">Da biste grupu sustava Microsoft 365 sakrili da bude vidljiva klijentima sustava Exchange, koristite sljedeću naredbu u EXO ljuski:</span><span class="sxs-lookup"><span data-stu-id="704c2-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

