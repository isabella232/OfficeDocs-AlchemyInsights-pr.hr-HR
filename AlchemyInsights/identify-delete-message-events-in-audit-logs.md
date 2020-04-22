---
title: Prepoznavanje događaja brisanja poruka u zapisnicima nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716488"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Nadzor zapisnika za izbrisane poruke e-pošte

Počevši od siječnja 2019, Microsoft po zadanom uključuje zapisivanje nadzora poštanskog sandučića. U suprotnom, da biste pregledali događaje brisanja poruka za određenog korisnika, morate ručno omogućiti akcije brisanja za nadzor. Ako je zapisivanje nadzora poštanskog sandučića već omogućeno za vašu tvrtku ili ustanovu ili za određenog korisnika, slijedite korake u nastavku.

1. Prijava u Centar za [& sigurnosti sustava Microsoft 365](https://protection.office.com/)

2. Kliknite **Pretraživanje i istraživanje** i odaberite Pretraživanje **zapisnika nadzora**.

3. Odaberite datumski raspon u poljima **Datum početka** i **Datum završetka.** Navedite korisničko ime za korisnika kojeg želite istražiti (korisnika koji je izbrisao stavke). U polju **Aktivnosti** odaberite **Izbrisane poruke iz mape Izbrisane stavke** i **Premještene poruke u mapu Izbrisane stavke**.

4. Kliknite **Pretraživanje**.

U rezultatima odaberite zapis nadzora. U potpaleti pojedinosti kliknite **Dodatne informacije**. Dodatne informacije o izbrisanoj stavci (na primjer, retku predmeta i mjestu artikla prilikom brisanja) prikazuju se u polju **ZahvaćeniArtikli.** Svojstvo **ClientInfoString** prikazat će se je li došlo do brisanja u programu Outlook, programu Outlook na webu (ranije poznatom kao Outlook Web App) ili bilo kojem drugom uređaju.

Dodatne informacije potražite u [odjeljku Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Napomena:** Izbrisane stavke ne možete dohvatiti pomoću značajke zapisnika nadzora. Da biste dohvatili izbrisane poruke u programu Outlook na webu, [pročitajte članak Oporavak izbrisanih stavki u web-aplikaciji Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
