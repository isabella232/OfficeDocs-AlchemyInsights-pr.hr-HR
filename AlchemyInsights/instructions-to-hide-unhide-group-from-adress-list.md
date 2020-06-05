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
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580001"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Sakrij grupu microsoft 365 s popisa adresa (GAL)

Da biste sakrili grupu sustava Microsoft 365 s popisa adresa (GAL) klijenata sustava Exchange (kao što su Outlook ili OWA), koristite sljedeću naredbu u EXO ljuski:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Da biste grupu Microsoft 365 sakrili od vidljivosti klijentima sustava Exchange, koristite sljedeću naredbu u EXO ljuski:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

