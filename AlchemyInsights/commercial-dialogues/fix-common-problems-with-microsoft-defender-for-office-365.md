---
title: Rješavanje uobičajenih problema s programom Microsoft Defender za Office 365
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
ms.openlocfilehash: 9104615baa5bf6dc91468912168e42ece6727eadd5330f1eb34e2a9170568b26
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898236"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Rješavanje uobičajenih problema s programom Microsoft Defender za Office 365

Evo nekoliko rješenja najčešćih problema s programom Microsoft Defender za Office 365:

- **Kašnjenje poruke:**

  Kašnjenja u isporuci e-pošte mogu uzrokovati Sef pregledavanjem poruka privici. Dodatne informacije potražite u članku [Sef postavke pravilnika privici](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Izvješće o lažno pozitivnim ili negativnim rezultatima:**

  Dodatne informacije potražite u članku [Prijava poruka i datoteka Microsoftu](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Omogući zaštitu Sef veza:**

  1. Na portalu Microsoft 365 Defender u odjeljku E-pošta & pravila <https://security.microsoft.com/>  \> **suradnje & Pravila** \>  \> **prijetnji Sef veze** u **odjeljku Pravila.**

     Da biste se izravno Sef **veze,** koristite <https://security.microsoft.com/safelinksv2> .

  2. Na **stranici Sef veze** odaberite pravilnik klikom na naziv pravilnika.
  3. U letak s detaljima koji će se prikazati učinite nešto od sljedećeg:
     - Da biste dodali novi pravilnik, odaberite **+ Stvori**. Pokrenut će se čarobnjak koji će vam pomoći da definirate postavke pravilnika.
     - Da biste uredili postojeći pravilnik, odaberite pravilnik klikom na naziv pravilnika. U brošuri s detaljima koja će se prikazati **odaberite Uređivanje** u **odjeljku Postavke** zaštite.
  4. Na **stranici Postavke** zaštite konfigurirajte sljedeće postavke:
     - Uključite **mogućnost Odaberite akciju za nepoznate potencijalno zlonamjerne URL-ove u porukama**.
     - Odaberite **Primijeni sigurne veze na poruke poslane unutar tvrtke ili ustanove**.

  Dodatne informacije potražite u članku [Postavljanje pravilnika Sef veza u programu Microsoft Defender za Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
