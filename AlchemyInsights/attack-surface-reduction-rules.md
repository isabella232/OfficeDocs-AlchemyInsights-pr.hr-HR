---
title: Pravila smanjivanja površine napada
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676071"
---
# <a name="attack-surface-reduction-rules"></a>Pravila smanjivanja površine napada

Izuzimanje datoteka i mapa može ozbiljno smanjiti zaštitu koju pružaju pravila smanjenja površine napada. Datoteke koje bi pravilo blokiralo dopušteno je pokretanje i ne snima se izvješće ni događaj. Iznimka se primjenjuje na sva pravila koja dopuštaju izuzimanja.

Asr izuzimanja koriste istu sintaksu kao i Microsoft Defender Antivirus izuzimanja. Detalje potražite u članku [Konfiguriranje i provjera valjanosti izuzimanja za Microsoft Defender Antivirus skeniranja](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). Da biste izbjegli probleme, pregledajte [uobičajene pogreške koje želite izbjeći prilikom definiranja izuzimanja.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Ne podržavaju sva pravila ASR-a izuzimanja. Da biste provjerili podržava li pravilo izuzimanja, pogledajte pravila smanjenja [površine napad.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Pravila smanjivanja površine napada

Površina za napad tvrtke ili ustanove obuhvaća sva mjesta na kojima napadač može ugroziti uređaje ili mreže tvrtke ili ustanove. Smanjivanje površine napada znači zaštitu uređaja i mreže tvrtke ili ustanove, što napadačima ostavlja manje načina izvođenja napada. Konfiguriranje pravila smanjenja površine napada u programu Microsoft Defender za krajnju točku može vam pomoći.

Dodatne informacije potražite u sljedećim člancima:

- [Mapiranje GUID pravila ASR-a u naziv](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Preduvjeti pravila ZA ASR:
    - [Windows 10 Pro, verzija 1709 ili novija](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, verzija 1709 ili novija](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Poslužitelj, verzija 1803 (polugodišnji kanal) ili novija](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Prepoznavanje ispravnog izuzetog sadržaja koji je moguće primijeniti

1. Potražite ID događaja 1121 ili 1122 u zapisniku microsoft-Windows-Windows Defender/Operativni zapisnik.

1. Procijenite scenarij blokiranja i kontekst te potvrdite da je taj scenarij potrebno deblokirati.

1. U detaljima događaja pročitajte vrijednost Put, koja je vrijednost koja definira izuzimanje.
    - Izuzimanje učinite što je moguće strožim.
    - Ako je potrebno, primijenite zamjenski znak (na primjer, zamijenite varijablu korisnika).

1. Primijenite izuzimanje prema potrebama implementacije. Detalje potražite u članku [Prilagodba pravila smanjivanja površine napada](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>Izuzimanje nije počašćeno

1. Odredite podržava li pravilo izuzimanja. Detalje potražite u članku Napad [pravila smanjenja površine](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Pregledajte primijenjena izuzimanja i provjerite s podacima o događaju za pogreške ili pogrešno protumačiti zamjenske znakove. Dodatne informacije potražite u članku [Podržane vrste izuzimanja](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. ako je učinak pravila previsok, razmislite o premještanju pravila (natrag) u način nadzora da biste izvršili daljnju provjeru valjanosti. Detalje potražite u članku [Testiranje načina na koji Microsoft Defender za značajke krajnjih točaka funkcionira u načinu rada za nadzor](/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. Prikupite podatke o podršci da biste otvorili slučaj podrške pomoću ove naredbe:
    
   ** MDEClientAnalyzer.cmd -v**

    Dodatne informacije potražite u članku [Problemi s uređajem za unošenje na Microsoft Defender za krajnje točke](issues-with-onboarding-machines.md).
