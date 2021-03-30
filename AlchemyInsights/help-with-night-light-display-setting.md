---
title: Pomoć za postavku prikaza noćog svjetla
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404265"
---
# <a name="help-with-the-night-light-display-setting"></a>Pomoć za postavku prikaza noćog svjetla

Dodatne informacije o postavkama noćnog prikaza potražite u članku Postavljanje prikaza za [noćno vrijeme u sustavu Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Ako su mogućnosti noćnog svjetla zasivljene u odjeljku Postavke, provjerite upravljački program za prikaz: 

1. Kliknite okvir za pretraživanje na programskoj traci i upišite **Upravitelj uređaja**, a zatim u **rezultatima pretraživanja** odaberite Upravitelj uređaja.
1. Proširite **odjeljak Prilagodnici za prikaz**. 

Značajka noćnih svjetiljki nažalost nije dostupna ako uređaj koristi upravljački program DisplayLink ili upravljački program za osnovni zaslon.

Značajka noćnog svjetla koristi nedavno korištenu grafičku tehnologiju, pa ćete možda morati ažurirati upravljački program za prikaz:  

- Provjerite ima li ažuriranja tako da **otvorite Start**  >  **Settings**  >  **Update & sigurnosna** provjera ažuriranja za Windows  >    >  **Update**.  

OR

- Posjetite web-mjesto za podršku proizvođača hardvera da biste ručno preuzeli i instalirali najnovije upravljačke programe za prikaz.

## <a name="reset-night-light-in-the-registry"></a>Ponovno postavljanje noćnog svjetla u registru

Ako ažuriranje upravljačkog programa za prikaz ne funkcionira, možda ćete morati ponovno postaviti noćno svjetlo u registru.  

**Oprez:** Ovaj se korak za otklanjanje poteškoća preporučuje samo naprednim korisnicima. Ako nepravilno izmijenite registar, može doći do ozbiljnih problema. Radi dodatne zaštite sigurnosno kopiranje registra prije izmjene da biste ga mogli vratiti ako se pojave problemi.

1. U okvir za pretraživanje upišite **regedit**, a zatim u **rezultatima pretraživanja** odaberite Uređivač registra.

1. Idite na sljedeći ključ registra: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Izvoz i brisanje sljedećeg potključa:$$windows.data.bluelightreduction.bluelightreductionstate

1. Izvoz i brisanje sljedećeg potključa:$$windows.data.bluelightreduction.settings

1. Ponovno pokrenite Windows i provjerite jesu li dostupne mogućnosti noćnog svjetla.


