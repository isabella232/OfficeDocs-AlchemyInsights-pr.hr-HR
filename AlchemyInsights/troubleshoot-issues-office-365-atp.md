---
title: Rješavanje problema s Office 365 Napredno prijetnja zaštite (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030912"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Rješavanje problema s Office 365 ATP

- **Kašnjenja obavijest s isporuka poruka e-pošte**? Pokušajte koristeći mogućnost dinamičke isporuke za pravila ATP sigurnom privitke. To će izbjeći kašnjenja dostave poruka e-pošte dok primatelji Zaštita od zlonamjernih datoteke.
- **Želite li izvješće positives false ili false Negacija**? Koristite ovu vezu za slanje datoteka za analizu:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Jeste li znali možete omogućiti veze sigurnom ATP zaštitu e-pošte poslane između osobe u vašoj organizaciji**? Slijedite ove korake:
    1. Idi na https://protection.office.com, i prijavite se.
    2. Idi na **Upravljanje prijetnja** > **pravila** > **Sigurne veze**.
    3. Pod **pravila koje se odnose na određene primatelje**uređivanje (ili dodavanje) pravila.
    4. Odaberite **Primijeni sigurnom veze poruke šalju unutar organizacije**.
    5. Spremite pravilo i dopustiti otprilike 30 minuta za promjene rad njihove način kroz vaš datacenter.
- Da biste dobili pomoć s ATP, pogledajte [Office 365 Napredno prijetnja zaštita](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).