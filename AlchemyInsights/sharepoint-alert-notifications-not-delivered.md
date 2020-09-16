---
title: Obavijesti o upozorenjima u sustavu SharePoint nisu isporučene
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751235"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Obavijesti o upozorenjima u sustavu SharePoint nisu isporučene

Potvrdite mapu BEZVRIJEDNA pošta u poruci e-pošte, kao što se ponekad može pojaviti upozorenje.

Odredite hoće li se **sva upozorenja isporučiti** ili ako se ne dostavi **pojedinačna upozorenja** iz određene datoteke ili biblioteke.

- **Pojedinačna upozorenja ne isporučuju**se: ako se pojedinačno upozorenje iz određene datoteke ili biblioteke ne dostavi, možete je pokušati izbrisati i ponovno stvoriti. Pogledajte odjeljak [Upravljanje, prikaz i brisanje upozorenja sustava SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) da biste ponovno stvorili upozorenje.
- **Sva se upozorenja ne isporučuju**: ako se ne isporučuju sva upozorenja iz više datoteka ili biblioteka, posjetite [nadzornu ploču zdravstvenog](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) sustava da biste provjerili ima li nekih savjeta/incidenata koji se događaju u sustavu SharePoint ili sustavu Exchange. Problem može biti uz mogućnost upozorenja sustava SharePoint ili kašnjenja u porukama e-pošte putem sustava Exchange. Važno je i napomenuti je li druga e-pošta isporučena, a ako ne, problem je vjerojatno s odgodama u sustavu Exchange.

Najčešća pitanja o upozorenjima:

- Nije moguće uputiti upozorenja u grupu za raspodjelu, podržane su samo sigurnosne i O365 grupe.
- Predloške e-pošte za upozorenje nije moguće prilagoditi; Da biste to postigli, potrebno je koristiti Microsoft FLOW ili tijek rada sustava SharePoint Designer.

## <a name="related-topics"></a>Srodne teme

Želite li isprobati Microsoft Flow u sustavu SharePoint Online?

- [Stvaranje toka](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint i Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
