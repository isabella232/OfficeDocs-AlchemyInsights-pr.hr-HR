---
title: Bitlocker ključevi za oporavak
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
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060056"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Pristup bitlocker ključevima za oporavak

Prilikom konfiguriranja postavki značajke Bitlocker Pravilnik o zaštiti krajnjih točaka u sustavu Intune moguće je definirati trebaju li se bitlocker podaci o oporavku pohraniti u Azure Active Directory.

Ako je ta postavka konfigurirana, pohranjeni podaci o oporavku moraju biti vidljivi administratoru aplikacije Intune kao dio podataka zapisa uređaja na oštrici Intune Devices na dva načina:

Uređaji – uređaji Azure AD -> "Device" OR Devices -> All Devices -> "Device" -> Recovery keys

Osim toga, ako postoji administrativni pristup samom uređaju, ključ za oporavak (lozinka) može se vidjeti pokretanjem sljedeće naredbe iz povišenog naredbenog retka:

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
Ako je uređaj šifriran prije uključivanja u Intune, ključ oporavka možda je povezan s "Microsoftovim računom" (MSA) koji se koristi za prijavu na uređaj tijekom postupka OOBE. Ako je to bio slučaj, pristup msa-u i prijava pomoću tog MSA-a trebao bi  https://onedrive.live.com/recoverykey prikazati uređaje za koje su pohranjeni ključevi za oporavak.
 
Ako je uređaj šifriran kao rezultat konfiguracije putem pravilnika grupe utemeljenog na domeni, podaci o oporavku mogu se pohraniti u lokalnom servisu Active Directory.

Ako ste konfigurirali pravilnik zaštite krajnjih točaka da biste ključ oporavka pohranjili u Azure Active Directory, ali ključ za određeni uređaj nije prenesen, prijenos možete pokrenuti zakretanjem ključa za oporavak za taj uređaj s MEM konzole. Detalje potražite u članku [Rotiranje BitLocker ključeva za oporavak](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

