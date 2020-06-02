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
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508980"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Zapisnici nadzora za izbrisane poruke e-pošte

Počevši od siječnja 2019. U suprotnom, da biste pregledali događaje brisanja poruka za određenog korisnika, morate ručno omogućiti akcije brisanja za nadzor. Ako je zapisivanje nadzora poštanskog sandučića već omogućeno za vašu tvrtku ili ustanovu ili za određenog korisnika, slijedite korake u nastavku.

1. Prijavite se u Centar za [usklađenost sa sigurnosnim & sustava Microsoft 365](https://protection.office.com/)

2. Kliknite **Pretraživanje i istraživanje** i odaberite Pretraživanje **zapisnika nadzora**.

3. Odaberite datumski raspon u poljima **Datum početka** i **Datum završetka.** Navedite korisničko ime za korisnika koje želite istražiti (korisnika koji je izbrisao stavke). U polju **Aktivnosti** odaberite **Izbrisane poruke iz mape Izbrisane stavke** i **Premještene poruke u mapu Izbrisane stavke**.

4. Kliknite **Pretraži**.

U rezultatima odaberite zapis nadzora. U potpaleti pojedinosti kliknite **Dodatne informacije**. Dodatne informacije o izbrisanoj stavci (na primjer, redak predmeta i mjesto stavke kada je izbrisana) prikazuju se u polju **Zahvaćeneite.** Svojstvo **ClientInfoString** prikazat će se je li brisanje došlo u programu Outlook, Outlook na webu (ranije poznat kao Outlook Web App) ili bilo kojem drugom uređaju.

Dodatne informacije potražite [u odjeljku Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Napomena:** izbrisane stavke ne možete dohvatiti pomoću značajke zapisnika nadzora. Da biste dohvatili izbrisane poruke u programu Outlook na webu, pročitajte članak [Oporavak izbrisanih stavki u web-aplikaciji Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
