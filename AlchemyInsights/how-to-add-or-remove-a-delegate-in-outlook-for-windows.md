---
title: Dodavanje i uklanjanje delegata u programu Outlook za Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573304"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Dodavanje i uklanjanje delegata u programu Outlook za Windows

Da biste dodali delegata u programu Outlook za Windows, učinite sljedeće: 

1. Kliknite karticu **datoteka** , a zatim **Postavke računa**, a zatim odaberite **pristup delegiranju**.
2. Kliknite **Dodaj**. Ako se **Dodavanje** ne prikazuje, aktivna veza možda ne postoji između programa Outlook i sustava Exchange. Traka stanja programa Outlook prikazuje status veze.
3. Upišite ime osobe koju želite označiti kao delegat ili pretražite i odaberite naziv na popisu rezultata pretraživanja.

    > [!NOTE]
    > Delegat mora biti osoba na globalnom popisu adresa sustava Exchange tvrtke ili ustanove (GAL).
4. Kliknite **Dodaj** , a zatim **u redu**.
5. U dijaloškom okviru **dozvole delegata** prihvatite zadane postavke dozvola ili odaberite prilagođene razine pristupa za mape sustava Exchange.

    - Ako delegatu treba dozvola za rad samo sa zahtevima za sastanak i odgovorima, zadane postavke dozvola, kao što je **delegira, primaju kopije poruka vezanih uz sastanak poslane meni** su dovoljne. Postavku dozvola **ulazne pošte** možete ostaviti na servisu **none**. Zahtjevi za sastanak i odgovori izravno će doći do ulazne pošte delegata.

    > [!NOTE]
    > Delegat je po zadanom odobren za **urednika (može čitati, stvarati i mijenjati stavke)** u mapu **kalendara** . Kada delegira sastanak u vaše ime, on se automatski dodaje u mapu **kalendara** .

5. Da biste slali poruku da biste obavijestili delegata o promijenjenim dozvolama, potvrdite okvir **automatski šalji poruku delegiranju sažetka tih dozvola** .
6. Ako želite, potvrdite okvir **delegat može vidjeti moje privatne stavke** .

    > [!IMPORTANT]
    > Ta postavka utječe na sve mape sustava Exchange. To obuhvaća sve mape pošta, kontakti, kalendar, zadaci, bilješke i dnevnik. Pristup privatnim stavkama ne može se omogućiti samo u navedenim mapama.

7. Odaberite **u redu**.

    > [!NOTE]
    >
    > - Poruke poslane s **dozvolama za slanje** u ime obuhvaćaju i delegate i vaša imena pokraj pošiljatelja. Kada se poruka pošalje s dozvolama za slanje kao, prikazat će se samo vaše ime.
    > - Kada nekoga dodate kao delegata, možete dodati poštanski sandučić sustava Exchange u njegov profil programa Outlook. Upute potražite u članku [Upravljanje stavkama pošte i kalendara neke druge osobe](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Da biste uklonili delegata u programu Outlook za Windows, učinite sljedeće:

1. Kliknite karticu **datoteka** .
2. Kliknite **Postavke računa** , a zatim **pristupite delegiranju**.
3. Odaberite naziv delegata za kojeg želite promijeniti dozvole, a zatim kliknite **Ukloni** , a zatim **u redu**.
