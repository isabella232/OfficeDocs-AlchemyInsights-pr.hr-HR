---
title: DLP možda treba prilagođenu vrstu
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030786"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP možda treba prilagođenu vrstu

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP može zahtijevati prilagođenu vrstu podataka**

Uz pravilnik o sprječavanju gubitka podataka (DLP) možete prepoznati i zaštititi osjetljive podatke u tvrtki ili ustanovi. U nekim scenarijima možda ćete morati stvoriti vlastitu **prilagođenu** osjetljivu vrstu podataka da biste zaštitili podatke tvrtke ili ustanove.

Vaša će tvrtka ili ustanova, primjerice, morati prepoznati i zaštititi ID-ove zaposlenika ili druge podatke u nekom obliku specifičnom za vašu organizaciju. Ako je tako, dodatne informacije potražite u sljedećim člancima.
  
 **Prilagodba ugrađene osjetljive vrste podataka**
  
Ako bi ugrađena vrsta osjetljivih podataka zadovoljila vaše potrebe uz samo nekoliko ugađanja, možete prilagoditi [ugrađenu osjetljivu vrstu podataka](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Možete, primjerice, dodavati ili uklanjati ključne riječi ili dodavati ili uklanjati popratne dokaze kao što su datum ili adresa.
  
 **Stvaranje prilagođene osjetljive vrste podataka**
  
No ako morate u potpunosti prepoznati i zaštititi drugu vrstu osjetljivih podataka, možete stvoriti prilagođenu [osjetljivu](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) vrstu podataka u UI-ju centra za & usklađenost.
  
**Stvaranje prilagođene osjetljive vrste podataka u programu PowerShell centra & sigurnosti**

Naposljetku, ako UI ne nudi sve potrebne mogućnosti, možete stvoriti prilagođenu osjetljivu vrstu podataka u [odjeljku Sigurnost & usklađenosti PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Počevši od XML datoteke, možete koristiti sve dostupne mogućnosti.
