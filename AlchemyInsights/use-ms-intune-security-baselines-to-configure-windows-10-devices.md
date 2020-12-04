---
title: Konfiguriranje uređaja sa sustavom Windows 10 pomoću Microsoft Intune sigurnosne osnove
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
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573298"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Konfiguriranje uređaja sa sustavom Windows 10 pomoću Microsoft Intune sigurnosne osnove

Umetanje sigurnosnih osnovnih stranica olakšava zaštitu korisnika i uređaja. Sigurnosne osnove sustava Windows postavke su prije konfigurirane grupe koje se koriste za primjenu poznate grupe postavki i zadanih vrijednosti koje preporučuje relevantni sigurnosni timovi. Stvaranjem profila sigurnosnog osnovnog sustava u programu Intune stvara se predložak koji se sastoji od više profila za konfiguraciju uređaja.

Kada implementirate sigurnosne osnovice na grupe korisnika ili uređaja, postavke se primjenjuju na uređaje koji se pokreću u sustavu Windows 10 ili novijim verzijama. Na primjer, MDM sigurnost Baseline automatski (1) omogućuje BitLocker za uklonjive pogone, (2) potrebna je lozinka za otključavanje uređaja i (3) onemogućuje osnovnu provjeru autentičnosti. Kada zadana vrijednost ne funkcionira u vašem okruženju, prilagodite osnovicu da biste primijenili postavke koje su vam potrebne.

Sigurnosni bazelini također pomažu u osnivanju krajnje sigurnog tijeka rada u programu Microsoft 365. Slijede neke prednosti ovog:

- Sigurnosno osnovica obuhvaća najbolje prakse i preporuke za postavke koje utječu na sigurnost. Budući da je Intune Partners s timom za sigurnost sustava Windows koji stvara osnovice za pravila grupe, ove se preporuke temelje na čvrstim smjernicama i opsežnom iskustvu.
- Ako ste novi u Intune i niste sigurni gdje početi, onda će vam sigurnosne osnove pomoći da brzo stvorite i implementirate siguran profil.
- Ako trenutno koristite pravilo grupe, zatim Migriranje u potrebe za upravljanjem znatno je jednostavnije uz sigurnosne osnovice, jer su ugrađene u Intune i obuhvaćaju najmodernije mogućnosti za upravljanje.

Dodatne informacije potražite u članku [sigurnosne osnove sustava Windows](https://go.microsoft.com/fwlink/?linkid=2141503) i [Upravljanje mobilnim uređajima](https://go.microsoft.com/fwlink/?linkid=2141701).