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
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930967"
---
# <a name="active-directory-not-syncing"></a>Active Directory se ne sinkronizira

Ako primate pogreške sinkronizacije, kao što je "bez nedavne sinkronizacije" ili primijetite status sinkronizacije direktorija na portalu za administratore sustava Office kaže: "Last synced more than 3 days ago" (Zadnje sinkronizirano prije više od 3 dana) možda AADConnect ima netočne postavke ili nedovoljne dozvole za izvođenje sinkronizacije.  

Ponovna instalacija AADConnect pomoću ekspresnih postavki može brzo riješiti problem:

1. [Preuzmite najnoviju verziju servisa AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Slijedite upute za ekspresne instalacije](/azure/active-directory/hybrid/how-to-connect-install-express).

Servis Azure AD Connect mora biti instaliran na poslužitelju Windows Server 2012 ili novijoj verziji. Ovaj poslužitelj mora biti spojen na domenu i može biti kontroler domene ili poslužitelj člana. Potpuni popis preduvjeta za Azure AD Povezivanje preduvjeta i preduvjeta pregledajte [Preduvjeti](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)za Azure AD Povezivanje .

Dodatne informacije o računima servisa AADConnect potražite u članku [Azure AD Povezivanje: Računi i dozvole](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
