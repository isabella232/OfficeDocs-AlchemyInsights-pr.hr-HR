---
title: Konfiguriranje Microsoft Intune sigurnosnih osnovica za Windows 10 uređaje
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104336"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Konfiguriranje Microsoft Intune sigurnosnih osnovica za Windows 10 uređaje

Intune sigurnosne osnovne vrijednosti štite korisnike i uređaje. Sigurnosne osnovne vrijednosti Windows unaprijed konfigurirane grupe postavki koje se koriste za primjenu poznate grupe postavki i zadanih vrijednosti koje preporučuju odgovarajući sigurnosni timovi. Stvaranjem sigurnosnog osnovnog profila u aplikaciji Intune stvarate predložak koji se sastoji od više profila konfiguracije uređaja.

Prilikom implementacije sigurnosnih osnovica grupama korisnika ili uređaja postavke se primjenjuju na uređaje koji se Windows 10 novije verzije. Na primjer, MDM Security Baseline automatski (1) omogućuje BitLocker za uklonjive pogone, (2) zahtijeva lozinku za otključavanje uređaja, a (3) onemogućuje osnovnu provjeru autentičnosti. Kada zadana vrijednost ne funkcionira za vaše okruženje, prilagodite osnovnu vrijednost da biste primijenili potrebne postavke.

Sigurnosne osnovice pomažu i pri uspostavi sigurnog tijeka rada s kraja na Microsoft 365. U nastavku su neke od prednosti ovog:

- Sigurnosna osnovica obuhvaća najbolje prakse i preporuke za postavke koje utječu na sigurnost. Budući da intune partneri s Windows sigurnosnim timom koji stvaraju osnovne vrijednosti za pravilnike grupe, te se preporuke temelje na čvrstim smjernicama i opsežnom iskustvu.
- Ako ste novi u programu Intune i niste sigurni gdje početi, sigurnosne osnovne vrijednosti pomoći će vam da brzo stvorite i implementite siguran profil.
- Ako trenutno koristite pravilnik grupe, migriranje u Intune radi upravljanja mnogo je jednostavnije uz sigurnosne osnovice jer su ugrađene u Intune i obuhvaćaju vrhunske mogućnosti upravljanja.

Dodatne informacije potražite u članku [Windows i](https://go.microsoft.com/fwlink/?linkid=2141503) upravljanje [mobilnim uređajima](https://go.microsoft.com/fwlink/?linkid=2141701).