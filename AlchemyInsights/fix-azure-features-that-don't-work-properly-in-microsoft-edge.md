---
title: Što učiniti ako značajke sustava Azure ne funkcioniraju pravilno u aplikaciji Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117080"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Što učiniti ako značajke sustava Azure ne funkcioniraju pravilno u aplikaciji Microsoft Edge

Microsoft Edge ima [poznate probleme](https://go.microsoft.com/fwlink/?linkid=2140608) povezane sa sigurnosnim zonama i mogu utjecati na to kako se korisnici servisa Azure prijav Windows centar za administratore. Ako imate poteškoća s korištenjem značajki sustava Azure Microsoft Edge, učinite sljedeće:

1. Na **izborniku Start** potražite internetske **mogućnosti i** odaberite je.
2. U **dijaloškom okviru Internetska** svojstva otvorite **karticu** Sigurnost.
3. Odaberite **zonu Pouzdana** web-mjesta, a zatim gumb **Web-mjesta.**
4. U **dijaloškom okviru Pouzdana** web-mjesta dodajte URL pristupnika, a [https://login.microsoftonline.com](https://login.microsoftonline.com) zatim [https://login.live.com](https://login.live.com) odaberite **Zatvori**.
5. U **dijaloškom okviru Internetska** svojstva otvorite **karticu Zaštita** privatnosti.
6. U **odjeljku Blokator skočnih prozora** odaberite **Postavke**. U dijaloškom okviru koji će se otvoriti dodajte URL pristupnika, a [https://login.microsoftonline.com](https://login.microsoftonline.com) zatim [https://login.live.com](https://login.live.com) odaberite **Zatvori**.
