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
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820278"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="904b2-102">Pristup bitlocker ključevima za oporavak</span><span class="sxs-lookup"><span data-stu-id="904b2-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="904b2-103">Prilikom konfiguriranja postavki značajke Bitlocker Pravilnik o zaštiti krajnjih točaka u sustavu Intune moguće je definirati trebaju li se podaci o oporavku značajke Bitlocker pohraniti na servisu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="904b2-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="904b2-104">Ako je ta postavka konfigurirana, pohranjeni podaci o oporavku moraju biti vidljivi administratoru aplikacije Intune kao dio podataka zapisa uređaja na oštrici Intune Devices na dva načina:</span><span class="sxs-lookup"><span data-stu-id="904b2-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="904b2-105">Uređaji – uređaji Azure AD -> "Device" OR Devices -> All Devices -> "Device" -> Recovery keys</span><span class="sxs-lookup"><span data-stu-id="904b2-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="904b2-106">Osim toga, ako postoji administrativni pristup samom uređaju, ključ za oporavak (lozinka) može se vidjeti pokretanjem sljedeće naredbe iz povišenog naredbenog retka:</span><span class="sxs-lookup"><span data-stu-id="904b2-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="904b2-107">Ako je uređaj šifriran prije uključivanja u Intune, ključ oporavka možda je povezan s "Microsoftovim računom" (MSA) koji se koristi za prijavu na uređaj tijekom postupka OOBE.</span><span class="sxs-lookup"><span data-stu-id="904b2-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="904b2-108">Ako je to bio slučaj, pristup msa-u i prijava pomoću tog MSA-a trebao bi  https://onedrive.live.com/recoverykey prikazati uređaje za koje su pohranjeni ključevi za oporavak.</span><span class="sxs-lookup"><span data-stu-id="904b2-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="904b2-109">Ako je uređaj šifriran kao rezultat konfiguracije putem pravilnika grupe utemeljenog na domeni, podaci o oporavku mogu se pohraniti u lokalnom servisu Active Directory.</span><span class="sxs-lookup"><span data-stu-id="904b2-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="904b2-110">Ako ste konfigurirali pravilnik za zaštitu krajnjih točaka da biste ključ oporavka pohranjili na servisu Azure Active Directory, ali ključ za određeni uređaj nije prenesen, prijenos možete pokrenuti zakretanjem ključa za oporavak za taj uređaj s MEM konzole.</span><span class="sxs-lookup"><span data-stu-id="904b2-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="904b2-111">Detalje potražite u članku [Rotiranje BitLocker ključeva za oporavak](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="904b2-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

