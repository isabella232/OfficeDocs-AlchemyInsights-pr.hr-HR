---
title: Konfiguriranje uređaja sa sustavom Windows 10 pomoću Microsoft Intune sigurnosne osnove
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50692904"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Korištenje Microsoftovih sigurnosnih osnovnih stranica za konfiguriranje uređaja sa sustavom Windows 10

Umetanje sigurnosnih osnovnih stranica olakšava zaštitu korisnika i uređaja. Sigurnosne osnove sustava Windows postavke su prije konfigurirane grupe koje se koriste za primjenu poznate grupe postavki i zadanih vrijednosti koje preporučuje relevantni sigurnosni timovi. Stvaranjem profila sigurnosnog osnovnog sustava u programu Intune stvara se predložak koji se sastoji od više profila za konfiguraciju uređaja.

Kada implementirate sigurnosne osnovice na grupe korisnika ili uređaja, postavke se primjenjuju na uređaje koji se pokreću u sustavu Windows 10 ili novijim verzijama. Primjerice, sigurnosno osnovica za upravljanje Microsoftovim mobilnim uređajima (MDM) automatski (1) omogućuje BitLocker za uklonjive pogone, (2) potrebna je lozinka za otključavanje uređaja i (3) onemogućuje osnovnu provjeru autentičnosti. Kada zadana vrijednost ne funkcionira u vašem okruženju, možete prilagoditi osnovicu da biste primijenili postavke koje su vam potrebne.

Sigurnosni bazelini također pomažu u osnivanju krajnje sigurnog tijeka rada u programu Microsoft 365. Slijede neke prednosti ove funkcionalnosti:
- Sigurnosno osnovica obuhvaća najbolje prakse i preporuke za postavke koje utječu na sigurnost. Budući da je Intune Partners s timom za sigurnost sustava Windows koji stvara osnovice za pravila grupe, ove se preporuke temelje na čvrstim smjernicama i opsežnom iskustvu.
- Ako ste novi u Intune i niste sigurni gdje početi, onda će vam sigurnosne osnove pomoći da brzo stvorite i implementirate siguran profil.
- Ako trenutno koristite pravilo grupe, zatim Migriranje u potrebe za upravljanjem znatno je jednostavnije uz sigurnosne osnovice, jer se te sigurnosne osnove ugrađuju u Intune i obuhvaćaju najmodernije mogućnosti za upravljanje.

Dodatne informacije potražite u članku [sigurnosne osnove sustava Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) i [Upravljanje mobilnim uređajima](https://docs.microsoft.com/windows/client-management/mdm/).