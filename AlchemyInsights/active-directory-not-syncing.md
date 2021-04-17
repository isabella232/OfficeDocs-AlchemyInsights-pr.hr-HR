---
title: Active Directory se ne sinkronizira
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822843"
---
# <a name="active-directory-not-syncing"></a>Active Directory se ne sinkronizira

Ako primate pogreške sinkronizacije, kao što je "bez nedavne sinkronizacije" ili primijetite status sinkronizacije direktorija na portalu za administratore sustava Office, kaže: "Last synced more than 3 days ago" (Zadnje sinkronizirano prije više od 3 dana) može biti da AADConnect ima netočne postavke ili nedovoljne dozvole za izvođenje sinkronizacije.  

Ponovna instalacija AADConnect pomoću ekspresnih postavki može brzo riješiti problem:

1. [Preuzmite najnoviju verziju servisa AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Slijedite upute za ekspresne instalacije](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Dodatne informacije o računima servisa AADConnect potražite u članku [Azure AD Connect: Računi i dozvole](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
