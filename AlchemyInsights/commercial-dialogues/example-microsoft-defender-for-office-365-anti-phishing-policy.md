---
title: Primjer Pravilnika o Office 365 Microsoft Defender za zaštitu od krađe identiteta
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034998"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Primjer Pravilnika o Office 365 Microsoft Defender za zaštitu od krađe identiteta

Te postavke omogućuju pravilnik pod nazivom *Domena i izvršni direktor*. Ovaj pravilnik pruža zaštitu korisnika i domene od oponašanja, a zatim primjenjuje pravilnik na sve poruke e-pošte koje su primili korisnici unutar domene. Najprije dodajte sljedeće informacije da biste stvorili pravilnik:

- **Naziv:** Domain and CEO **Description:** Ensures that the CEO and your domain are not beingersonated.
  **Primijenjeno na**: **Odaberite domenu primatelja**. U **odjeljku Bilo koji od** tih mogućnosti **odaberite Odaberite**, a zatim odaberite domenu. Odaberite **+ Dodaj**. Potvrdite okvir pokraj naziva domene na popisu (na *primjer,* contoso.com ), a zatim odaberite **Dodaj**. Odaberite **Gotovo**.
- Nakon stvaranja pravilnika pravilnik možete precizno podesiti pomoću sljedećih mogućnosti:
  - **Dodavanje korisnika radi zaštite:** U ovom primjeru dodajte barem adresu e-pošte izvršnog direktora.
  - **Dodavanje domena radi zaštite:** dodajte domenu tvrtke ili ustanove koja obuhvaća ured glavnog direktora.
  - **Odaberite akcije**: **ako** e-poštu šalje oponašani korisnik , odaberite Preusmjeri poruku **na** drugu adresu e-pošte , a zatim unesite adresu e-pošte sigurnosnog administratora *(npr. securityadmin@contoso.com).* Ako **poruku e-pošte šalje oponašana domena**, odaberite **Karantena poruke**.
  - **Inteligencija poštanskog** sandučića : ta je mogućnost po zadanom odabrana kada stvorite novi pravilnik za zaštitu od krađe identiteta. Ostavite tu postavku **na radi** najboljih rezultata.
  - **Dodavanje pouzdanih pošiljatelja i domena:** U ovom primjeru nemojte definirati nadjačavanja.
- Kada pregledate postavke, odaberite Stvori **ovaj** pravilnik ili **Spremi**, prema potrebi.

Dodatne informacije potražite u članku Pravila za [zaštitu od krađe identiteta u Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
