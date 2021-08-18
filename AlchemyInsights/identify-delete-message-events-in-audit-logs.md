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
ms.openlocfilehash: f5d6041fd80b4d5cae610e7d9248e45ed410a3d9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317586"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Zapisnici nadzora za izbrisane poruke e-pošte

Počevši od siječnja 2019., Microsoft po zadanom uključuje zapisivanje nadzora poštanskog sandučića. U suprotnom, da biste pregledali događaje brisanja poruka za određenog korisnika, morate ručno omogućiti akcije brisanja za nadzor. Ako je zapisivanje nadzora poštanskog sandučića već omogućeno za vašu organizaciju ili određenog korisnika, slijedite korake u nastavku.

1. Prijavite se u centar [za Microsoft 365 usklađenost](https://protection.office.com/)

2. Kliknite **Pretraživanje i istraživanje pa** odaberite Pretraživanje **zapisnika nadzora**.

3. Odaberite raspon datuma u poljima **Datum početka** **i Datum** završetka. Navedite korisničko ime za korisnika koji želite istražiti (korisnika koji je izbrisao stavke). U polju **Aktivnosti odaberite** Izbrisane **poruke iz mape Izbrisane stavke i** **Premještene poruke u mapu Izbrisane stavke**.

4. Kliknite **Pretraživanje**.

U rezultatima odaberite zapis nadzora. U letci s pojedinostima kliknite **Dodatne informacije**. Dodatne informacije o izbrisanoj stavci (na primjer, retku predmeta i mjestu stavke kada je izbrisana) prikazuju se u polju **Zahvaćeniitami.** Svojstvo **ClientInfoString pokazat** će je li došlo do brisanja u Outlook, Outlook na webu (prijašnjeg naziva Outlook Web App) ili na bilo kojem drugom uređaju.

Dodatne informacije potražite u članku [Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Napomena:** izbrisane stavke ne možete dohvatiti pomoću značajke zapisnika nadzora. Da biste izbrisali izbrisane poruke Outlook webu, pogledajte oporavak [izbrisanih stavki u programu Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
