---
title: Stvaranje ulova e-pošte
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816192"
---
# <a name="create-an-email-catch-all"></a>Stvaranje ulova e-pošte

Korištenje ulova sve je jako obeshrabreno. Bolje je vratiti pošiljatelja da zna da se njihova poruka ne može isporučiti kao adresa da bi mogli poduzeti akciju. Možete i ograničiti nadzirani poštanski sandučić tako da ulovi samo prijašnje valjane adrese e-pošte. 

Svaki ulov svih poštanskih sandučića primit će mnogo neželjene pošte i naposljetku će se možda popuniti ako se ne nadzire. (Postoje ograničenja primanja.) 

Ako odlučite nastaviti, slijedite ove korake:

1. Stvaranje grupe za dinamičku raspodjelu & "Sve vrste primatelja".

2. Stvorite namjenski poštanski sandučić da biste uhvatili poruke e-pošte, catchall@domain.com.

3. Za određenu domenu postavite DomainType na "InternalRelay". Ako kasnije uklonite sve ulov, obavezno vratite domenu na Mjerodavno.

4. Stvorite pravilo prijenosa tijeka pošte na sljedeći način:

    - Ako je pošiljatelj "Outside the Organization" (Izvan tvrtke ili ustanove)
    - Preusmjeravanje poruke na Catchall@domain.com
    - Osim ako je primatelj član grupe allusers@domain.com (grupa za raspodjelu sadrži sve članove)
    - Provjerite jesu li novi poštanski sandučići dodani u grupu za dinamičku raspodjelu
