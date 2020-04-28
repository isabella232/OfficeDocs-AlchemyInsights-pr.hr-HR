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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skrivanje grupe za Microsoft 365 s popisa adresa (GAL)

Da biste sakrili grupu sustava Microsoft 365 s popisa adresa (GAL) klijenata sustava Exchange (kao što su Outlook ili OWA), koristite sljedeću naredbu u EXO ljuski:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Da biste grupu sustava Microsoft 365 sakrili da bude vidljiva klijentima sustava Exchange, koristite sljedeću naredbu u EXO ljuski:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

