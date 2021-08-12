---
title: Što učiniti ako značajke sustava Azure ne funkcioniraju pravilno u aplikaciji Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812862"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Što učiniti ako značajke sustava Azure ne funkcioniraju pravilno u aplikaciji Microsoft Edge

Microsoft Edge ima poznate probleme vezane uz sigurnosne zone koje mogu utjecati na način na koji se korisnici servisa Azure prijav Windows centar za administratore. Dodatne informacije potražite u članku [Poznati problemi na edgeu](https://go.microsoft.com/fwlink/?linkid=2140608). Ako imate poteškoća s korištenjem značajki servisa Azure Microsoft Edge, pokušajte sljedeće:

1. Na Izbornik Start na traci **za pretraživanje** upišite **Internetske mogućnosti,** a zatim je odaberite.
1. U **odjeljku Internetska** svojstva **odaberite karticu** Sigurnost.
1. Odaberite **Pouzdana web-mjesta**, a zatim **Web-mjesta**.
1. Dodajte URL pristupnika, kao i i <https://login.microsoftonline.com> <https://login.live.com> , a zatim odaberite **Zatvori**.
1. U **odjeljku Internetska** svojstva odaberite **karticu** Zaštita privatnosti.
1. U odjeljku Blokator skočnih prozora odaberite **Postavke**. Dodajte URL pristupnika, kao i , <https://login.microsoftonline.com> <https://login.live.com> a zatim odaberite **Zatvori**.