---
title: Izradite e-mail catch sve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286061"
---
# <a name="create-an-email-catch-all"></a>Izradite e-mail catch sve

Korištenje ulova sve je snažno obeshrabreno. Bolje je pružiti povrat natrag pošiljatelju ostavljajući pošiljateljima do znanja da se njihova poruka ne može isporučiti kako bi mogli poduzeti radnje. Nadzirani poštanski sandučić možete ograničiti i tako da uhvati samo ranije valjane adrese e-pošte. 

Svaki ulov sve poštanski sandučić će dobiti mnogo spam i svibanj na kraju ispuniti ako ne i pomno pratiti. (Postoje ograničenja primanja.) 

Ako odlučite nastaviti, slijedite ove korake:

1. Stvaranje grupe za dinamičku raspodjelu & uključuju "Sve vrste primatelja".

2. Izradite namjenski poštanski sandučić za ulak za e-poštu, na primjer catchall@domain.com.

3. Za određenu domenu postavite DomainType na "InternalRelay". Ako kasnije uklonite ulov sve, budite sigurni da postavite domenu natrag na autoritativno.

4. Kreirajte pravilo prijenosa tijeka pošte na sljedeći način:

    - Ako je pošiljatelj "Izvan organizacije"
    - Preusmjeravanje poruke na Catchall@domain.com
    - Osim ako je primatelj član allusers@domain.com (Grupa raspodjele sadrži sve članove)
    - Provjera valjanosti dodavanja novih poštanskih sandučića u grupu za dinamičku raspodjelu
