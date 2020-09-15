---
title: BitLocker ključevi oporavka
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
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685878"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Pristup tipkama za oporavak značajke BitLocker

Kada konfigurirate postavke zaštite značajke šifriranja krajnje točke, moguće je definirati hoće li se BitLocker informacije o oporavku pohraniti u servisu Azure Active Directory.

Ako je ta postavka konfigurirana, pohranjeni podaci o oporavku trebali bi biti vidljivi administratore kao dio podataka o zapisu uređaja u aplikaciji Intune Devices na dva načina:

Uređaji-Azure AD Devices-> "uređaj" ili uređaji-> svi uređaji-> "uređaj"-> tipke za oporavak

Alternativno, ako postoji administrativni pristup samom uređaju, ključ oporavka (lozinka) može se vidjeti pokretanjem sljedeće naredbe iz povišenog naredbenog upita:

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
Ako je uređaj bio šifriran prije upisa u programu Intune, ključ oporavka možda je povezan s "Microsoftovim računom" (MSP-om) koji se koristi za prijavu na uređaj tijekom postupka OOBE. Ako je to bio slučaj, pristup  https://onedrive.live.com/recoverykey i prijava s MSP-om trebao bi prikazati uređaje za koje su pohranjeni ključevi za oporavak.
 
Ako je uređaj bio šifriran kao rezultat konfiguracije putem pravilnika grupe utemeljenih na domeni, podaci o oporavku mogu biti spremljeni u servisu Active Directory.
 

