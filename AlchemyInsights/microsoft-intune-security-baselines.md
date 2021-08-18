---
title: Konfiguriranje Microsoft Intune sigurnosnih osnovica za Windows 10 uređaje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 911c6b1860e4f44e6d88897f73173cdd11060562
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331977"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Konfiguriranje Microsoft Intune sigurnosnih osnovica za Windows 10 uređaje

Intune sigurnosne osnovne vrijednosti štite korisnike i uređaje. Sigurnosne osnovne vrijednosti Windows unaprijed konfigurirane grupe koje se koriste za primjenu poznate grupe postavki i zadanih vrijednosti koje preporučuju odgovarajući sigurnosni timovi. Stvaranjem sigurnosnog osnovnog profila u aplikaciji Intune stvarate predložak koji se sastoji od više profila konfiguracije uređaja.

Kada sigurnosne osnovice implementirate u grupe korisnika ili uređaja, postavke se primjenjuju na uređaje koji se Windows 10 novijim verzijama. Na primjer, sigurnosna osnovica za upravljanje Microsoftovim mobilnim uređajima (MDM) automatski omogućuje BitLocker za uklonjive pogone, zahtijeva lozinku za otključavanje uređaja i onemogućuje osnovnu provjeru autentičnosti. Kada zadana vrijednost ne funkcionira za vaše okruženje, možete prilagoditi osnovnu vrijednost da biste primijenili potrebne postavke.

Sigurnosne osnovne vrijednosti pomažu i u uspostavi sigurnog tijeka rada s kraja na Microsoft 365. Osnovna sigurnosna osnovica obuhvaća najbolje prakse i preporuke za postavke koje utječu na sigurnost. Intune partneri s Windows sigurnosnim timom koji stvara osnovne vrijednosti za pravilnike grupe, pa se te preporuke temelje na čvrstim smjernicama i opsežnom iskustvu.

Ako ste novi u programu Intune i niste sigurni gdje početi, sigurnosne osnovne vrijednosti pomoći će vam da brzo stvorite i implementite siguran profil. Ako trenutno koristite pravilnik grupe, migriranje u Intune u svrhe upravljanja mnogo je jednostavnije uz sigurnosne osnovne vrijednosti jer su ugrađene u Intune i obuhvaćaju vrhunske mogućnosti upravljanja.

Dodatne informacije potražite u članku [Windows i](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) upravljanje [mobilnim uređajima](https://docs.microsoft.com/windows/client-management/mdm/).

