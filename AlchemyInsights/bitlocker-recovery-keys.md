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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="cee5f-102">Pristupanje BitLocker ključevima oporavka</span><span class="sxs-lookup"><span data-stu-id="cee5f-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="cee5f-103">Kada konfigurirate BitLocker postavke pravila zaštite mjera ishoda, moguće je definirati da li BitLocker informacije o oporavku treba pohraniti u Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cee5f-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="cee5f-104">Ako je ta postavka konfigurirana, spremljeni podaci o oporavku trebali bi biti vidljivi Intune admin-u kao dio podataka o zapisu uređaja u oštrici Intune Devices na dva načina:</span><span class="sxs-lookup"><span data-stu-id="cee5f-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="cee5f-105">Uređaji-Azure AD uređaji-> "uređaj" ili uređaji-> svi uređaji-> "uređaj"-> tipke za oporavak</span><span class="sxs-lookup"><span data-stu-id="cee5f-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="cee5f-106">Alternativno, ako postoji administrativni pristup samom uređaju, ključ oporavka (lozinka) može se vidjeti pokretanjem sljedeće naredbe iz povišenog naredbenog retka:</span><span class="sxs-lookup"><span data-stu-id="cee5f-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="cee5f-107">Ako je uređaj šifriran prije upisa u Intune, ključ oporavka možda je povezan s "Microsoftovim računom" (MSA) koji se koristi za prijavu na uređaj tijekom OOBE procesa.</span><span class="sxs-lookup"><span data-stu-id="cee5f-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="cee5f-108">Ako je to slučaj, pristup https://onedrive.live.com/recoverykey i prijava s tom MSA treba prikazati uređaje za koje su pohranjeni ključevi za oporavak.</span><span class="sxs-lookup"><span data-stu-id="cee5f-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="cee5f-109">Ako je uređaj šifriran kao rezultat konfiguracije putem pravila grupe koja se temelji na domeni, informacije o oporavku mogu se pohraniti u lokalni Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cee5f-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

