---
title: Upute za skrivanje/uklanjanje grupe s popisa adresa
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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768906"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Sakrij Office 365 grupu s popisa adresa (GAL)

Da biste sakrili grupu sustava Office 365 s popisa adresa (GAL) klijenata sustava Exchange (kao što su Outlook ili OWA), upotrijebite sljedeću naredbu u EXO ljusci:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Da biste sakrili grupu sustava Office 365 da bude vidljiva klijentima sustava Exchange, upotrijebite sljedeću naredbu u EXO ljusci:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

