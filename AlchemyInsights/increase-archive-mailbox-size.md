---
title: 305 Povećanje veličine arhive poštanskog sandučića
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f9cc968aba32645fd4433616618d096231ce4899e9e93335e802af5c05524a79
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926375"
---
# <a name="increase-the-archive-mailbox-size"></a>Povećanje veličine arhiviranja poštanskog sandučića


Ako želite da pokrenemo automatske provjere postavki navedenih u nastavku, odaberite gumb natrag < – pri vrhu ove stranice, a zatim unesite adresu e-pošte korisnika kojima je potrebna povećana veličina poštanskog sandučića arhive.

Microsoft 365 [ograničava](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) veličinu arhivskih poštanskih sandučića na temelju licence dodijeljene korisničkom računu. Kada arhivski poštanski sandučić dosegne 90 % dopuštene veličine, korisnik će primiti obavijest e-poštom. Kada arhivski poštanski sandučić dosegne ograničenje veličine, korisnik ne može premjestiti više stavki u arhivski poštanski sandučić. Microsoft 365 neće povećati veličinu arhivnog poštanskog sandučića nakon što se dosegne ograničenje veličine. Umjesto toga, korisnici mogu poduzeti sljedeće radnje da bi osloboditi prostor u arhiviranom poštanskom sandučiću:

- Izvoz stavki u .pst datoteku pomoću Outlook.

- Brisanje stavki iz arhive poštanskog sandučića.

Microsoft 365 **neograničeno arhiviranje za** Office 365 Enterprise E3 i E5. Administrator mora omogućiti tu značajku prije nego što poštanski sandučić u arhivi dosegne maksimalnu veličinu. Kada je omogućeno neograničeno arhiviranje, u arhivski poštanski sandučić može biti potrebno i do 30 dana. Stoga preporučujemo da administratori provjere slobodni prostor u arhiviranom poštanskom sandučiću, što korisniku omogućuje nastavak korištenja arhivskog poštanskog sandučića dok se proširuje. Dodatne informacije potražite u članku [Pregled neograničenog arhiviranja](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) u programu Microsoft 365 omogućivanje [neograničenog arhiviranja u Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

Dodatne informacije o pristupu arhiviranom poštanskom sandučiću iz Outlook potražite u članku Outlook za pristup stavkama [u automatski proširenoj arhivi](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Da biste konfigurirali pravilnik o zadržavanju koji automatski premješta stavke u arhivski poštanski sandučić, pogledajte članak Postavljanje pravilnika arhiviranja i brisanja poštanskih [sandučića u Microsoft 365 tvrtki ili ustanovi](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Napomena:** automatsko proširivanje arhiva nije podržano za primarne poštanske sandučiće u Exchange 2010.
