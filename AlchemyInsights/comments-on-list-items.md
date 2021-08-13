---
title: Komentari na stavke popisa
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
- "9003821"
- "6841"
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995469"
---
# <a name="comments-on-list-items"></a>Komentari na stavke popisa

Korisnici mogu pregledavati sve komentare na stavci popisa i filtrirati prikaze koji prikazuju komentare ili aktivnosti povezane s stavkom.

Korisnici moraju imati na umu sljedeće da bi mogli dodavati i brisati komentare:

- Komentari slijede postavke dozvola svojstvene sustavu SharePoint.
- Klasični popisi koji još nisu ugrađeni za prikaz u modernim korisničkim sučeljima, kao što su popisi zadataka, neće imati tu značajku komentiranja.
- Komentiranje popisa u aplikaciji Teams nije dostupno u ovom izdanju.
- Pretraživanje ne indeksiraju komentare.

Administratori tu značajku mogu onemogućiti na razini tvrtke ili ustanove promjenom parametra **CommentsOnListItemsDisabled** u **cmdletu Set-SPOTenant** PowerShell.

Trenutno nije moguće onemogućiti komentiranje na razini web-mjesta ili popisa. Nadamo se da ćemo te kontrole imati u kasnijem ažuriranju, vjerojatno u prvom tromjesečju 2021.
