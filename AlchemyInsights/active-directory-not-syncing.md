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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889210"
---
# <a name="active-directory-not-syncing"></a>Active Directory se ne sinkronizira

Ako primate pogreške sinkronizacije, kao što je "nema nedavne sinkronizacije" ili na portalu za administratore sustava Office primijetite status sinkronizacije direktorija, "Last synced more than 3 days ago" (Zadnje sinkronizirano prije više od 3 dana) može biti da AADConnect ima netočne postavke ili nedovoljne dozvole za izvođenje sinkronizacije.  

Ponovna instalacija sustava AADConnect pomoću ekspresnih postavki može brzo riješiti problem:

1. [Preuzmite najnoviju verziju servisa AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Slijedite upute za ekspresne instalacije](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Servis Azure AD Connect mora biti instaliran na poslužitelju Windows Server 2012 ili novijoj verziji. Ovaj poslužitelj mora biti spojen na domenu i može biti kontroler domene ili poslužitelj člana. Potpuni popis preduvjeta za Azure AD Povezivanje preduvjete i preduvjete pregledajte [Preduvjeti za Azure AD Povezivanje](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Dodatne informacije o računima servisa AADConnect potražite u članku [Azure AD Povezivanje: Računi i dozvole](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
