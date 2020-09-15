---
title: Prepoznavanje događaja za brisanje poruka u evidenciji nadzora
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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696505"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Zapisnici nadzora za izbrisane poruke e-pošte

Počevši od siječnja 2019, Microsoft će po zadanom uključiti evidentiranje nadzora poštanskih sandučića. U suprotnom, da biste pregledali brisanje događaja poruke za određenog korisnika, morate ručno omogućiti postupke brisanja za nadzor. Ako je zapisivanje nadzornog sandučića već omogućeno za vašu tvrtku ili ustanovu ili za određenog korisnika, slijedite upute u nastavku.

1. Prijavite se u [centar za sigurnost & sustava Microsoft 365](https://protection.office.com/)

2. Kliknite **pretraživanje i istraživanje** te odaberite **pretraživanje zapisnika nadzora**.

3. Odaberite raspon datuma u poljima **Datum početka** i **Datum završetka** . Navedite korisničko ime za korisnika koje želite istražiti (korisnik koji je izbrisao stavke). U polju **aktivnosti** odaberite **izbrisane poruke iz mape Izbrisane stavke** i **premjestite poruke u mapu Izbrisane stavke**.

4. Kliknite **Pretraživanje**.

U rezultatima odaberite zapis nadzora. U nastavku pojedinosti kliknite **više informacija**. Dodatne informacije o izbrisanoj stavci (na primjer, redak predmeta i mjesto stavke kada je izbrisana) prikazuju se u polju **Afecteditems** . Svojstvo **Clientinfostring** prikazat će se ako je brisanje došlo u programu Outlook, Outlook na webu (prethodno poznat kao Outlook Web App) ili bilo koji drugi uređaj.

Dodatne informacije potražite u članku [određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Pažnja**: izbrisane stavke ne možete dohvatiti pomoću značajke zapisnika nadzora. Upute za dohvaćanje izbrisanih poruka u programu Outlook na webu potražite [u članku Oporavak izbrisanih stavki u web-aplikaciji programa Outlook](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
