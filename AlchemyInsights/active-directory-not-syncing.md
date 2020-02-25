---
title: Active Directory ne sinkronizira
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265153"
---
# <a name="active-directory-not-syncing"></a>Active Directory ne sinkronizira

Ako primate pogreške pri sinkronizaciji, kao što je "bez nedavne sinkronizacije" ili primijetite status sinkronizacije direktorija na portalu za administratore sustava Office, kaže: "Zadnji put sinkroniziranprije više od 3 dana", možda AADConnect ima netočne postavke ili nedovoljne dozvole za izvođenje sinkronizacije.  

Ponovna instalacija aadconnecta pomoću ekspresnih postavki može brzo riješiti problem:

1. [Preuzmite najnoviju verziju AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Slijedite upute za brzu instalaciju](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Dodatne informacije o računima servisa AADConnect potražite u [odjeljku Povezivanje sa servisom Azure: Računi i dozvole](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
