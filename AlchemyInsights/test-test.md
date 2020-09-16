---
title: Uvjeti koje nema u trgovini termina sustava SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750443"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućivanje šifriranja BitLocker pomoću značajke Intune

Pravilnik o zaštiti krajnjih točaka može se koristiti za konfiguriranje postavki šifriranja za BitLocker za uređaje sa sustavom Windows, kao što je opisano u odjeljku: Windows10 (i novije) postavke za zaštitu uređaja pomoću aplikacije Intune

Morate biti svjesni da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko šifriranje šifriranja koje se pokreće bez primjene pravilnika MDM-a. To može utjecati na primjenu Pravilnika ako su konfigurirane standardne postavke. Dodatne pojedinosti potražite u članku Najčešća pitanja.


FAQ   Q: koja izdanja sustava Windows podržava šifriranje uređaja pomoću pravilnika o zaštiti krajnjih točaka?
 A: postavke u pravilu zaštite krajnjih točaka implementiraju se pomoću značajke BitLocker CSP-a.Ne podržavaju sva izdanja ni verzije sustava Windows pomoću značajke BitLocker CSP. 
      U ovom trenutku izdanja sustava Windows: Enterprise; Podržani su edukacijski, mobilni, mobilni Enterprise i Professional (od međuverzija 1809 prema dalje).




P: ako je uređaj već šifriran uz BitLocker pomoću zadanih postavki OS-a za metodu šifriranja i čvrstoću šifriranja (XTT-AIS-128) primjenjuje pravilo s drugim postavkama automatski pokreće ponovnu šifriranje pogona pomoću novih postavki?

O: Ne. Da bi se primijenile nove postavke šifre, pogon mora prvo biti dešifriran.

Podsjetnik za uređaje koji se upisuju uz autopilot automatsko šifriranje koje se događa tijekom programa OOBE nije pokrenuto dok se ne procjenjuje pravilo Intune koja omogućuje postavljanje postavki pravilnika koje se koriste umjesto zadanih vrijednosti OS-a.




Q ako je uređaj šifriran kao rezultat primjene pravilnika za Intune, hoće li se dešifrirati kada se to pravilo Ukloni?

O: uklanjanje šifriranja povezanog pravilnika ne rezultira dešifriranjem diskova koji su konfigurirani.




P: Zašto pravilnik o pridržavanju sukladnosti pokazuje da moj uređaj nema "omogućen BitLocker", ali jest?

A: postavka "omogućeno BitLocker" u pravilima za usklađenost s usklađenosti koristi klijent za zdravlje servisa Windows Device (ĐD). Ovaj klijent samo mjeri stanje uređaja u vremenu dizanja. Dakle, ako uređaj nije ponovno pokrenuto budući da je BitLocker enkripcija dovršen, servis za klijentski softver u programu ĐHA neće prijaviti BitLocker kao aktivan.