---
title: Upute za skrivanje/otkrivanje grupe s popisa adresa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926237"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skrivanje Microsoft 365 s popisa adresa (GAL)

Da biste sakrili Microsoft 365 iz popisa adresa (GAL) klijenata Exchange (kao što su Outlook ili OWA), u exo ljusci koristite sljedeću naredbu:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Da biste sakrili Microsoft 365 da bude vidljiva klijentima Exchange, u exo ljusci koristite sljedeću naredbu:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

