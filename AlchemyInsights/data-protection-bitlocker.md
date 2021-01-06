---
title: Zaštita podataka – BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768809"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućivanje šifriranja BitLocker pomoću značajke Intune

 Pravilnik o zaštiti krajnjih točaka može se koristiti za konfiguriranje postavki šifriranja BitLocker za uređaje sa sustavom Windows. Dodatne informacije potražite u članku [Postavke sustava Windows 10 (i novije) radi zaštite uređaja pomoću značajke Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Morate biti svjesni da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko šifriranje BitLocker šifriranja, koji se pokreće bez primjene pravilnika MDM-a. To može utjecati na primjenu Pravilnika ako su konfigurirane postavke koje nisu zadane. Dodatne pojedinosti potražite u sljedećim najčešća pitanja.
 
Informacije o otklanjanju poteškoća sa značajkom BitLocker potražite [u članku Otklanjanje poteškoća s značajkom BitLocker u programu Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Najčešća pitanja**

P: koja izdanja sustava Windows podržava šifriranje uređaja pomoću pravilnika o zaštiti krajnjih točaka?<br>
A: postavke u pravilu zaštite krajnjih točaka implementiraju se pomoću [značajke BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)-a. Ne podržavaju sva izdanja ili verzije sustava Windows pomoću značajke BitLocker CSP. <br><br>

P: kako BitLocker može biti omogućen na uređajima, a da ne zahtijeva interakciju krajnjih korisnika?<br>
O: dok god su ispunjeni neophodni predujmi, moguće je omogućiti BitLocker "Nečujnu enkripciju" putem programa Intune. Pojedinosti o zahtjevima uređaja i primjerima pravilnika o pravilniku omogućuju nečujno šifriranje u sljedećem dokumentu: [tiho Omogući šifriranje](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)šifriranja. <br><br>

P: ako je uređaj već šifriran uz BitLocker pomoću zadanih postavki OS-a za metodu šifriranja i čvrstoću šifriranja (XTT-AIS-128), hoće li primjena pravilnika s drugim postavkama automatski aktivirati ponovno šifriranje pogona pomoću novih postavki?<br>
O: Ne. Da biste primijenili nove postavke šifriranja, pogon mora prvo biti dešifriran.<br><br>
**Upozorenje:** Da bi se uređaji upisali kao autopilot, automatsko šifriranje koje bi se dogodilo tijekom programa OOBE ne pokreće se dok se ne procjenjuje pravilo Intune, što omogućuje postavljanje postavki temeljenih na pravilima na mjestu zadane vrijednosti OS-a.
 
P: ako je uređaj šifriran kao rezultat aplikacije Intune Policy, hoće li se dešifrirati kada se to pravilo Ukloni?<br>
A: uklanjanje pravilnika koje se odnose na šifriranje ne rezultira dešifriranjem diskova koji su konfigurirani.
 
P: Zašto pravilnik o pridržavanju sukladnosti pokazuje da moj uređaj nema omogućen BitLocker, čak i ako jest?<br>
A: postavka "omogućeno BitLocker" u politici usklađivanja usklađenosti koristi klijent sustava Windows za zdravlje attestation (ĐD). Ovaj klijent samo mjeri stanje uređaja u vremenu dizanja. Dakle, ako uređaj nije ponovno pokrenuto nakon dovršetka šifriranja BitLocker, servis servisa ĐHA Client neće prijaviti BitLocker kao aktivan.
 
 