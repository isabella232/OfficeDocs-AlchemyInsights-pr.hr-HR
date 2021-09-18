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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446683"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP možda treba prilagođenu vrstu

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP može zahtijevati prilagođenu vrstu podataka**

Uz pravilnik o sprječavanju gubitka podataka (DLP) možete prepoznati i zaštititi osjetljive podatke u tvrtki ili ustanovi. U nekim scenarijima možda ćete morati stvoriti vlastitu prilagođenu osjetljivu vrstu podataka da biste zaštitili podatke tvrtke ili ustanove. Dodatne informacije potražite u članku Informacije [o osjetljivim vrstama podataka i definicijama](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) [entiteta vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

Dodatne informacije o stvaranju prilagođenih osjetljivih vrsta podataka i pravilnika potražite u članku: 

**Prilagodba ugrađene osjetljive vrste podataka**

Ako bi ugrađena vrsta osjetljivih podataka zadovoljila vaše potrebe uz samo nekoliko ugađanja, pogledajte [prilagodba ugrađene osjetljive vrste podataka](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Možete, primjerice, dodavati ili uklanjati ključne riječi ili dodavati ili uklanjati popratne dokaze kao što su datum ili adresa.

**Stvaranje prilagođene osjetljive vrste podataka**

No ako morate u potpunosti prepoznati i zaštititi drugu vrstu osjetljivih podataka, možete stvoriti prilagođenu osjetljivu vrstu podataka u Centar za usklađenost okruženja Microsoft 365. Dodatne informacije potražite u članku Početak [rada s prilagođenim osjetljivim vrstama podataka](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).

**Stvaranje prilagođene osjetljive vrste podataka u programu PowerShell centra za & sigurnosti**

Naposljetku, ako korisničko sučelje ne nudi sve potrebne mogućnosti, možete stvoriti prilagođenu osjetljivu vrstu podataka u odjeljku PowerShell centra za sigurnost & usklađenosti. Počevši od XML datoteke, možete koristiti sve dostupne mogućnosti. Dodatne informacije potražite u članku [Stvaranje prilagođene osjetljive vrste podataka pomoću komponente PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

Da biste najprije testirajte pravilnik u testnom načinu rada, pogledajte implementaciju pravilnika u [testnom](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) načinu rada i Stvaranje, testiranje i [ugađanje pravilnika OLP-a](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy). 