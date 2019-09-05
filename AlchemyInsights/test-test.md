---
title: Uvjeti nedostaju iz spremišta termina Online SharePoint
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762045"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućivanja Bitlocker šifriranja s Intune

Pravila zaštite Intune krajnje točke mogu se konfigurirati postavke šifriranja Boitlocker za uređaje sustava Windows kao što je opisano u: Windows10 (i novijima) postavke za zaštitu uređaja pomoću Intune

Imajte na umu da mnogi uređaji novija izvodi Windows 10 podržava automatsko bitlocker šifriranje koje je pokrenulo bez aplikacije MDM pravila. Aplikacija pravila to utjecati ako konfigurirane postavke koje nisu zadane. Više detalja potražite u odjeljku najčešća pitanja vezana uz.


Najčešća pitanja vezana uz  Q: koje izdanjima sustava Windows podržava uređaj šifriranje pomoću pravila zaštite krajnja točka?
 A: postavke u pravilima zaštite krajnje točke Intune su implementirati pomoću Bitlocker CSP.Nisu sve izdanja niti izgradi Windows podržava Bitlocker CSP. 
      Na ovom vrijeme izdanja sustava Windows: Enterprise; Podržane su Obrazovanje, mobilni, mobilni Enterprise i Professional (iz build 1809 nadalje).




Q: Ako uređaj već šifriran pomoću Bitlocker koristeći zadane postavke OS za metodu šifriranja i snaga šifriranja (XTS-AES-128) će Primjena pravila s različitim postavkama automatski okidač ponovnog šifriranja pogona s nove postavke?

A: Br. Za primjenu nove postavke snaga moraju prvo dešifrirati pogon.

Napomena za uređaje koji se upisani s Autopilot automatsko šifriranje koje bi doći tijekom OOBE se aktivira dok Intune pravila vrednovanja koja omogućuje pravila temelji postavke koristiti umjesto zadanih postavki OS




Q ako uređaj šifrirani zbog aplikacije pravila Intune će ga se dešifrirati kada se uklone tog pravila?

A: uklanjanje šifriranja Srodni pravila rezultirati dešifriranje pogona koji su konfigurirani.




Q: Zašto se intune pravila usklađenosti ne Pokaži moj uređaj imaju "Omogućeno Bitlocker", ali je?

A: na "Bitlocker omogućeno" postavka pravila usklađenosti intune koristi klijent Windows uređaj stanja Attestation (DHA). Ovaj klijent samo mjeri stanje uređaja prilikom pokretanja. Tako ako uređaj ne sustava nakon dovršetka bitlocker šifriranje klijentski servis DHA će izvješće bitlocker kao aktivni.