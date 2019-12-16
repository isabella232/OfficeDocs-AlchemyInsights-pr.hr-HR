---
title: Uvjeti koji nedostaju iz spremišta termina SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053505"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućavanje BitLocker šifriranja s Intune

Intune pravilo zaštite sigurnosti može se koristiti za konfiguriranje postavke šifriranja Boitlocker za Windows uređaje kao što je opisano u: Windows10 (i noviji) postavke za zaštitu uređaja pomoću Intune

Trebali biste biti svjesni da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko BitLocker šifriranje koje se aktivira bez primjene MDM pravila. To može utjecati na primjenu pravila ako su konfigurirane nezadane postavke. Pogledajte FAQ za više detalja.


Često  postavljana pitanja Q: koja izdanja sustava Windows podržavaju šifriranje uređaja pomoću pravila o zaštiti krajnjih točaka?
 O: postavke u pravilima zaštite sigurnosti Intune provode se pomoću BitLocker CSP-a.Ne podržavaju sva izdanja ni verzije sustava Windows BitLocker CSP. 
      U ovom trenutku izdanja sustava Windows: Enterprise; Podržano je obrazovanje, Mobilno, Mobilno poduzeće i profesionalni (od izgradnje 1809 prema naprijed).




P: ako je uređaj već šifriran s BitLocker pomoću zadane postavke OS-a za metodu šifriranja i čvrstoću šifriranje (XTS-AES-128) će primijeniti pravilo s različitim postavkama automatski aktivirati ponovno šifriranje pogona s novim postavkama?

A: ne. Kako biste primijenili nove postavke šifriranja, pogon mora prvo biti dešifriran.

Napomena za uređaje koji se upisuje autopilotom automatsko šifriranje koje će se pojaviti tijekom OOBE ne pokreće se dok se ne ocijeni pravila Intune koja omogućuje postavljanje postavki utemeljenih na pravilima za zadane postavke operacijskog sustava




Q ako je uređaj šifriran kao rezultat primjene pravila Intune hoće li se dešifrirati kada se ta pravila uklone?

O: uklanjanje pravila povezanih s šifriranjem ne rezultira dekriptiranje diskova koji su konfigurirani.




P: Zašto neprecizno pravilo usklađenosti pokazuje da moj uređaj nema "BitLocker omogućen", ali je?

A: postavka "omogućeno za BitLocker" u pravilima usklađenosti koristi se s klijentskim programom za osiguranje sustava Windows (DHA). Ovaj klijent mjeri stanje uređaja samo u vrijeme pokretanja. Dakle, ako se uređaj nije ponovno pokrenuo jer je BitLocker šifriranje dovršen, usluga DHA klijenta neće prijaviti BitLocker kao aktivnu.