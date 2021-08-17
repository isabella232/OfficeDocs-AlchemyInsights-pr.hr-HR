---
title: Uvjeti koji nedostaju u trgovini SharePoint online trgovini terminima
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106407"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućivanje bitlocker šifriranja pomoću aplikacije Intune

Intune Endpoint Protection Policy može se koristiti za konfiguriranje postavki šifriranja značajke Boitlocker za Windows uređaje kao što je opisano u postavkama sustava : Windows10 (i noviji) radi zaštite uređaja pomoću aplikacije Intune

Imajte na umu da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko bitlocker šifriranje koje se pokreće bez primjene pravilnika MDM-a. To može utjecati na primjenu pravilnika ako nisu zadane postavke konfigurirane. Dodatne pojedinosti potražite u odjeljku Najčešća pitanja.


Najčešća pitanja Pitanja: koja izdanja Windows podržavaju šifriranje uređaja pomoću pravilnika o zaštiti krajnjih točaka?
O: Postavke pravilnika o zaštiti krajnjih točaka u aplikaciji Intune implementira se pomoću bitlocker CSP-a.  Ne podržavaju sva izdanja ni međuverzije Windows bitlocker CSP. U ovom trenutku Windows izdanja: Enterprise; Podržane su obrazovne, mobilne, mobilne i profesionalne tvrtke (od međuverzije 1809 nadalje).




P: Ako je uređaj već šifriran pomoću bitlockera pomoću zadanih postavki operacijskog sustava za način šifriranja i jačinu šifriranja (XTS-AES-128) primijenit će pravilnik s različitim postavkama automatski pokreće ponovno šifriranje pogona novim postavkama?

O: Ne. Da biste primijenili nove postavke šifriranja, pogon najprije morate dešifrirati.

Napomena Za uređaje koji se registriraju pomoću autopilota automatsko šifriranje koje bi se odvijalo tijekom OOBE-a ne pokreće se dok se ne procijeni Pravilnik o intuneu koji omogućuje korištenje postavki utemeljenih na pravilniku na mjestu zadanih postavki operacijskog sustava




Q Ako je uređaj šifriran zbog primjene pravilnika o intuneu, hoće li se dešifrirati kada se taj pravilnik ukloni?

O: Uklanjanje pravilnika povezanog s šifriranjem NE rezultira dešifriranje konfiguriranih pogona.




P: Zašto intune Compliance Policy pokazuje da moj uređaj nema "Bitlocker Enabled", ali jest?

O: Postavka "Bitlocker enabled" (Bitlocker omogućena) u pravilniku o usklađenosti intune koristi klijent Windows attestation (DHA). Taj klijent mjeri samo stanje uređaja u vrijeme pokretanja. Dakle, ako se uređaj nije ponovno pokrenuo od dovršetka bitlocker šifriranja, klijentski servis DHA neće prijaviti bitlocker kao aktivan.