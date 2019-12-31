---
title: BitLocker ključevi oporavka
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908807"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Pristupanje BitLocker ključevima oporavka

Kada konfigurirate BitLocker postavke pravila zaštite mjera ishoda, moguće je definirati da li BitLocker informacije o oporavku treba pohraniti u Azure Active Directory.

Ako je ta postavka konfigurirana, spremljeni podaci o oporavku trebali bi biti vidljivi Intune admin-u kao dio podataka o zapisu uređaja u oštrici Intune Devices na dva načina:

Uređaji-Azure AD uređaji-> "uređaj" ili uređaji-> svi uređaji-> "uređaj"-> tipke za oporavak

Alternativno, ako postoji administrativni pristup samom uređaju, ključ oporavka (lozinka) može se vidjeti pokretanjem sljedeće naredbe iz povišenog naredbenog retka:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Ako je uređaj šifriran prije upisa u Intune, ključ oporavka možda je povezan s "Microsoftovim računom" (MSA) koji se koristi za prijavu na uređaj tijekom OOBE procesa. Ako je to slučaj, pristup https://onedrive.live.com/recoverykey i prijava s tom MSA treba prikazati uređaje za koje su pohranjeni ključevi za oporavak.
 
Ako je uređaj šifriran kao rezultat konfiguracije putem pravila grupe koja se temelji na domeni, informacije o oporavku mogu se pohraniti u lokalni Active Directory.
 

