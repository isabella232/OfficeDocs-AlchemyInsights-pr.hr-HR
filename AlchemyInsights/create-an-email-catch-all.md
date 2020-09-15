---
title: Stvaranje e-pošte za hvatanje svih
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712978"
---
# <a name="create-an-email-catch-all"></a>Stvaranje e-pošte za hvatanje svih

Korištenje hvatanja sve se snažno obeshrabri. Bolje je vratiti pošiljatelju da pošalje pošiljatelja da zna da se poruka ne može isporučiti kao adresirana da bi mogla poduzeti akcije. Možete i ograničiti nadzirani poštanski sandučić samo da biste uhvatili prethodno valjane adrese e-pošte. 

Bilo koji ulov svi poštanski sandučić dobit će dobar dio neželjene pošte i eventualno može popuniti ako ne pomno prati. (Postoje ograničenja koja primate) 

Ako odlučite nastaviti, slijedite ove korake:

1. Stvaranje grupe za dinamičku raspodjelu & obuhvaća "sve vrste primatelja".

2. Stvorite namjenski poštanski sandučić da biste uhvatili poruke e-pošte, primjerice catchall@domain.com.

3. Za određene domene postavite domenu domena na "InternalRelay". Ako kasnije uklonite sve nalaze, obavezno ponovno postavite domenu na autoritativno.

4. Stvaranje pravila transporta e-pošte na sljedeći način:

    - Ako je pošiljatelj "izvan tvrtke ili ustanove"
    - Preusmjeravanje poruke na Catchall@domain.com
    - Osim ako je primatelj član allusers@domain.com (grupa za raspodjelu sadrži sve članove)
    - Provjerite jeste li potvrdili da se novi poštanski sandučići dodaju u grupu za dinamičku raspodjelu
