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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080738"
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
