---
title: Odredite Brisanje poruke događaja u zapisnika nadzora
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416702"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Evidencija nadzora za poruke e-pošte izbrisane

Početni 2019 siječanj, Microsoft je uključivanje zapisivanja po zadanom nadzor poštanskog sandučića. U suprotnom, za pregled brisanje poruka događaje za određenog korisnika, morate ručno omogućiti brisanje akcije za nadzor. Nadzor poštanskog sandučića zapisivanje već omogućeno za organizaciju ili za određenog korisnika, slijedite dolje navedene korake.

1. Prijavite se u sustav [Office 365 sigurnosne & usklađenosti centar](https://protection.office.com/)

2. Kliknite **za pretraživanje i istraživanja** i odaberite **Pretraživanje zapisnika nadzora**.

3. Odaberite raspon datum u polja **Datum početka** i **Datum završetka** . Navedite korisničko ime korisnika koji želite istražiti (korisnik koji izbrisane stavke). U polju **aktivnosti** odaberite **Izbrisane poruke iz mape Izbrisane stavke** i **Moved poruke u mapu Izbrisane stavke**.

4. Kliknite **Pretraži**.

U rezultatima, odaberite nadzora zapisa. Potpaleta pojedinosti kliknite **Dodatne informacije**. Dodatne informacije o izbrisana stavka (na primjer, redak predmeta i mjesto artikla kada je izbrisana) prikazuje se u polju **AffectedItems** . Svojstvo **ClientInfoString** će prikazati ako brisanja došlo je do u programu Outlook, Outlook na webu (nekadašnjeg naziva Outlook Web App) ili drugi uređaj.

Za dodatne informacije pogledajte [Determining tko postaviti poštanski sandučić za prosljeđivanje e-pošte](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Napomena**: nije moguće dohvatiti izbrisane stavke pomoću značajke zapisnika nadzora. Dohvatiti izbrisane poruke u programu Outlook na webu potražite [Oporavi izbrisane stavke u Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
