---
title: Slanje prilagođenih obavijesti pomoću aplikacije Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720638"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Upute za slanje prilagođenih obavijesti korisnicima upravljanih uređaja sa sustavom iOS i uređajima sa sustavom Android

Prilagođene obavijesti za Intune obrađuju aplikacija Portal tvrtke na korisnikovom uređaju. Aplikacija zatim stvara obavijesti o pritiskom na tom uređaju.

Slijede preduvjeti za uređaj da biste podržali primitak prilagođenih obavijesti, a da bi aplikacija stvorila obavijest o pritisku:

- Uređaj mora imati instaliranu aplikaciju Portal tvrtke.  

- Uređaj mora dopustiti aplikaciji Portal tvrtke da šalje obavijesti o pritiskom. Kada je aplikacija instalirana ili ažurirana, ona će zatražiti od korisnika da dozvoli obavijesti.

- Uređaji sa sustavom Android moraju imati instaliran Google Reproduciraj servise.

- Uređaj mora biti upisan pomoću aplikacije Intune.

Dodatne informacije, uključujući način slanja poruke, potražite u [dokumentaciji značajki](https://docs.microsoft.com/intune/custom-notifications).
