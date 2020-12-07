---
title: Što učiniti ako značajke Azure ne funkcioniraju pravilno u pregledniku Microsoft Edge
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
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583227"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Što učiniti ako značajke Azure ne funkcioniraju pravilno u pregledniku Microsoft Edge

Microsoft Edge sadrži [poznate probleme](https://go.microsoft.com/fwlink/?linkid=2140608) koji se odnose na sigurnosne zone i mogu utjecati na to kako se korisnici Azure prijave u centar za administratore sustava Windows. Ako imate problema s upotrebom značajki Azure s programom Microsoft Edge, isprobajte sljedeće korake:

1. Na izborniku **Start** potražite **mogućnosti interneta** i odaberite ga.
2. U dijaloškom okviru **internetska svojstva** otvorite karticu **Sigurnost** .
3. Odaberite zonu **pouzdanih web-mjesta** , a zatim odaberite gumb **web-mjesta** .
4. U dijaloškom okviru **pouzdana web-mjesta** Dodajte URL pristupnika, kao [https://login.microsoftonline.com](https://login.microsoftonline.com) i [https://login.live.com](https://login.live.com) , a zatim odaberite **Zatvori**.
5. U dijaloškom okviru **internetska svojstva** otvorite karticu **Zaštita privatnosti** .
6. U odjeljku **blokator skočnih prozora** odaberite **Postavke**. U dijaloškom okviru koji će se otvoriti Dodajte URL pristupnika, kao [https://login.microsoftonline.com](https://login.microsoftonline.com) i [https://login.live.com](https://login.live.com) , a zatim odaberite **Zatvori**.
