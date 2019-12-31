---
title: Data Protection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908702"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućavanje BitLocker šifriranja s Intune

 Intune pravila o zaštiti krajnjih točaka mogu se koristiti za konfiguriranje postavki BitLocker šifriranja za uređaje sa sustavom Windows. Dodatne informacije potražite u odjeljku [Postavke sustava Windows 10 (i noviji) kako biste zaštitili uređaje pomoću programa Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Trebali biste biti svjesni da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko BitLocker šifriranje, koje se aktivira bez primjene MDM pravila. To može utjecati na primjenu pravila ako su konfigurirane postavke koje nisu zadane. Dodatne pojedinosti potražite u sljedećim FAQ-u.
 
Informacije o rješavanju problema s BitLocker podacima potražite [u članku Otklanjanje poteškoća s BitLocker pravilima u programu Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Faq**

 P: koja izdanja sustava Windows podržavaju šifriranje uređaja pomoću pravila za zaštitu krajnjih točaka?<br>
 O: postavke u pravilima o zaštiti krajnjih točaka Intune provode se pomoću [BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)-a. Ne podržavaju sva izdanja ili verzije sustava Windows BitLocker CSP. <br><br>
      U ovom trenutku podržane su sljedeće izdanja sustava Windows: Enterprise, Education, Mobile, Mobile Enterprise i Professional (Build 1809 i noviji).
 
P: ako je uređaj već šifriran s BitLocker pomoću zadane postavke OS-a za metodu šifriranja i snagu šifriranja (XTS-AES-128), primijenit će pravila s različitim postavkama automatski aktivirati ponovno šifriranje pogona novim postavkama?<br>
A: ne. Da biste primijenili nove postavke šifriranja, pogon prvo mora biti dešifriran.<br><br>
**Napomena:** Za uređaje koji se upisuje autopilot, automatsko šifriranje koje će se pojaviti tijekom OOBE-a ne aktivira se dok se ne ocijeni pravila Intune, što omogućuje da se postavke temeljene na politici koriste umjesto zadanih postavki operacijskog sustava.
 
P: ako je uređaj šifriran zbog primjene pravila Intune, hoće li se dešifrirati kada se ta pravila uklone?<br>
A: uklanjanje pravila vezanih za šifriranje ne rezultira dešifriranjem diskova koji su konfigurirani.
 
P: Zašto pravila o sukladnosti Intune pokazuju da moj uređaj nije omogućen za BitLocker, iako je to?<br>
A: postavka "omogućena za BitLocker" u politici sukladnosti sustava pravilne uporabe koristi klijent za zdravlje uređaja za zdravstvenu potvrdu (DHA). Ovaj klijent mjeri stanje uređaja samo u vrijeme pokretanja. Dakle, ako se uređaj nije ponovno pokrenuo od dovršetka BitLocker šifriranja, usluga DHA klijenta neće prijaviti BitLocker kao aktivnu.
 
 