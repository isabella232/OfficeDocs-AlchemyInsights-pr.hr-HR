---
title: Implementacija aplikacije Win32 app
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461758"
---
# <a name="intune-win32-app-deployment"></a>Implementacija aplikacije Win32 app

Microsoft Intune omogućuje aplikacije Win32, uključujući, ali ne ograničavajući se na MSI i. EXE će se implementirati na uređajima sa sustavom Windows 10. Korišten je mehanizam implementacije da bi se na ciljnom uređaju prikazao proširenje (IME) za upravljanje. IME će se automatski instalirati kao rezultat ciljanja skripte za PowerShell ili programa Win32 na korisnika/uređaja.

Postoji i skup unaprijed obaveznih zahtjeva koji se moraju zadovoljiti da bi se implementirali Win32 aplikacije koje obuhvaćaju sljedeće:

- Podržane platforme: Windows 10 verzija 1607 ili novija (verzije poduzeća, Pro i obrazovne ustanove).
- Podržana arhitektura: x86 i x64.
- Upravljanje uređajima: AAD se pridružio i automatski upisuje (uključujući hibridnu domenu i pravila grupe automatski se upisuju).
- Oblik paketa aplikacija:. **intunewin**  datoteka koju priprema [alat za pripremu sadržaja u programu Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Ograničenja
    - Maksimalna veličina: 8GB.
    - Nepodržana arhitektura: ruke.

Pregledajte dokument "[Dodavanje, dodjeljivanje i praćenje aplikacije Win32 u programu Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" za informacije vezane uz te korake.

Pojedinosti o otklanjanju poteškoća prilikom implementacije aplikacija u sustavu Windows, uključujući aplikacije Win32, mogu se pregledati u sljedećim dokumentima

- [Otklanjanje poteškoća s instalacijom aplikacija](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Otklanjanje poteškoća s aplikacijama Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)