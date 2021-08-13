---
title: SharePoint obavijesti upozorenja nisu isporučene
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
ms.openlocfilehash: 05bd913098372a57d3061e8c516a6a6b4f0a9bdafde02acc930062d6281d06dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957893"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint obavijesti upozorenja nisu isporučene

Provjerite mapu BEZVRIJEDNO u poruci e-pošte jer ponekad upozorenja mogu biti tamo.

Odredite ne **isporučuju li se sva upozorenja** ili se **ne** isporučuju pojedinačna upozorenja iz određene datoteke ili biblioteke.

- **Pojedinačna se upozorenja ne isporučuju**: ako se ne isporučuje pojedinačno upozorenje iz određene datoteke ili biblioteke, možete ga pokušati izbrisati i ponovno stvoriti. Pogledajte [upravljanje, prikaz ili brisanje SharePoint upozorenja da](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) biste ponovno skončali upozorenje.
- **Sva se upozorenja ne isporučuju:** ako se ne isporučuju sva upozorenja iz više datoteka ili biblioteka, posjetite nadzornu ploču Stanje servisa da biste provjerili ima li kakvih upozorenja/incidenata koji se mogu pojaviti s SharePoint ili Exchange. [](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) Problem može biti s mogućnostima SharePoint upozorenja ili kašnjenjima u porukama e-pošte putem Exchange. Važno je i napomenuti isporučuje li se druga e-pošta, a ako ne, problem je vjerojatno Exchange kašnjenja.

Najčešća pitanja o upozorenjima:

- Nije moguće slati upozorenja grupi za raspodjelu, podržane su samo grupe sigurnost i O365.
- Ne možete prilagoditi predloške upozorenja e-pošte; da biste to postigli, morate koristiti Microsoft FLOW ili SharePoint designer workflow.

## <a name="related-topics"></a>Povezane teme

Želite li isprobati Microsoft Flow SharePoint online?

- [Stvaranje Flow](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint i Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
