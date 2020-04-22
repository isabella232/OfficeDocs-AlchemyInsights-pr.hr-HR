---
title: Pojmovi koji nedostaju u spremištu termina sustava SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766845"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućavanje Bitlocker šifriranja pomoću intune

Intune Endpoint Protection Policy može se koristiti za konfiguriranje BoitLocker postavki šifriranja za Windows uređaje kao što je opisano u : Postavke sustava Windows10 (i noviji) za zaštitu uređaja pomoću intune

Trebali biste biti svjesni da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko bitlocker šifriranje koje se pokreće bez primjene MDM pravila. To može utjecati na primjenu pravila ako su konfigurirane postavke koje nisu zadane. Pogledajte najčešća pitanja za više detalja.


Faq  P: Koja izdanja sustava Windows podržavaju šifriranje uređaja pomoću pravila zaštite krajnje točke?
 O: Postavke u pravilima zaštite krajnje točke intune implementiraju se pomoću Bitlocker CSP-a.Ne podržavaju sva izdanja ni međuverzije sustava Windows Bitlocker CSP. 
      U ovom trenutku Windows Izdanja: Enterprise; Obrazovanje, Koji se kreće, Koji se kreće Poduzeće i Koji se odnosi na zvanje ( from graditi 1809 nadalje) jesu podržanih od.




P: Ako je uređaj već šifriran s BitLocker pomoću zadanih postavki OS-a za metodu šifriranja i snagu šifriranja (XTS-AES-128) će primijeniti pravila s različitim postavkama automatski će pokrenuti ponovno šifriranje pogona s novim postavkama?

A: Ne. Da biste primijenili nove postavke šifriranja, pogon se najprije mora dešifrirati.

Napomena Za uređaje koji se upisuju s autopilotom automatsko šifriranje koje će se dogoditi tijekom oOBE-a ne pokreće se dok se ne procijeni intune pravilo koje omogućuje da se umjesto zadanih postavki osustavu OS koriste postavke utemeljene na pravilima.




Q Ako je uređaj šifriran kao rezultat primjene pravila intune će se dešifrirati kada se to pravilo ukloni?

O: Uklanjanje pravila vezanih uz šifriranje NE rezultira dešifrirati pogone koji su konfigurirani.




P: Zašto pravila usklađivanja s usklađenošću pokazuju da moj uređaj nema "Bitlocker omogućen", ali jest?

O: Postavka "Bitlocker omogućena" u pravilniku o usklađenosti u usklađivanju koristi klijent za provjeru stanja uređaja u sustavu Windows (DHA). Ovaj klijent mjeri samo stanje uređaja u vrijeme pokretanja. Dakle, ako uređaj nije ponovno podizanje sustava od bitlocker šifriranje je dovršen DHA klijent usluga neće prijaviti bitlocker kao aktivan.