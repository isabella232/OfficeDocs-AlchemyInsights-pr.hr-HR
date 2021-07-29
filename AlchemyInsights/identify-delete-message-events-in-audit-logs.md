---
title: Prepoznavanje događaja brisanja poruka u zapisnicima nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7dd9c98bd45c29702fbc6cc14bf82bf7bce7d89d
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630061"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Zapisnici nadzora za izbrisane poruke e-pošte

Počevši od siječnja 2019., Microsoft po zadanom uključuje zapisivanje nadzora poštanskog sandučića. U suprotnom, da biste pregledali događaje brisanja poruka za određenog korisnika, morate ručno omogućiti akcije brisanja za nadzor. Ako je zapisivanje nadzora poštanskog sandučića već omogućeno za vašu organizaciju ili za određenog korisnika, slijedite korake u nastavku.

1. Prijavite se u centar [za Microsoft 365 usklađenost](https://protection.office.com/)

2. Kliknite **Pretraživanje i istraživanje pa** odaberite Pretraživanje **zapisnika nadzora**.

3. Odaberite raspon datuma u poljima **Datum početka** **i Datum** završetka. Navedite korisničko ime za korisnika koji želite istražiti (korisnika koji je izbrisao stavke). U polju **Aktivnosti odaberite** **Izbrisane poruke iz mape Izbrisane stavke i** **Premještene poruke u mapu Izbrisane stavke**.

4. Kliknite **Pretraživanje**.

U rezultatima odaberite zapis nadzora. U letci s pojedinostima kliknite **Dodatne informacije**. Dodatne informacije o izbrisanoj stavci (primjerice, retku predmeta i mjestu stavke prilikom brisanja) prikazuju se u polju **Zahvaćeniotemi.** Svojstvo **ClientInfoString pokazat** će je li došlo do brisanja u Outlook, Outlook na webu (prijašnjeg naziva Outlook Web App) ili bilo kojeg drugog uređaja.

Dodatne informacije potražite u članku [Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Napomena:** izbrisane stavke ne možete dohvatiti pomoću značajke zapisnika nadzora. Da biste izbrisali izbrisane poruke Outlook webu, pogledajte oporavak [izbrisanih stavki u programu Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
