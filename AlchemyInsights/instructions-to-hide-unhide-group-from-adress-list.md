---
title: Upute za sakrivanje/otkrivanje grupe s popisa adresa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663001"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Sakrivanje grupe Microsoft 365 iz popisa adresa (GAL)

Da biste skrivali grupu Microsoft 365 iz popisa adresa (GAL) klijenata sustava Exchange (kao što su Outlook ili OWA), upotrijebite sljedeću naredbu u programu EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Da biste grupu Microsoft 365 skrivali od vidljivog prema klijentima sustava Exchange, upotrijebite sljedeću naredbu u programu EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

