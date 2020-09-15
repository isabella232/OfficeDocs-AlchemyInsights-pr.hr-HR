---
title: Active Directory nije sinkroniziranje
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697621"
---
# <a name="active-directory-not-syncing"></a>Active Directory nije sinkroniziranje

Ako primate pogreške pri sinkronizaciji, kao što je "Nema nedavne sinkronizacije" ili primijetite da status sinkronizacije direktorija na portalu za administratore sustava Office kaže: "zadnje sinkronizirano prije više od 3 dana", moguće je da AADConnect ima pogrešne postavke ili nedovoljne dozvole za izvođenje sinkronizacije.  

Ponovnim instalacijom servisa AADConnect pomoću ekspresne postavke možete brzo razriješiti problem:

1. [Preuzmite najnoviju verziju servisa AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Slijedite upute za ekspresne instalacije](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Dodatne informacije o računima servisa AADConnect potražite u članku [Azure ad Connect: računi i dozvole](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
