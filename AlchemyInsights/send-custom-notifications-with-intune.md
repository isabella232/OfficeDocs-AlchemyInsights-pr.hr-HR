---
title: Slanje prilagođenih obavijesti pomoću Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992305"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Kako slati prilagođene obavijesti korisnicima upravljanih iOS i Android uređaja

Prilagođene obavijesti za Intune obrađuju aplikacija Portal tvrtke na korisnikovom uređaju. Aplikacija zatim stvara push obavijest na tom uređaju.

Sljedeći su preduvjeti za uređaj za podršku primitka prilagođenih obavijesti, a za aplikaciju zatim stvoriti push obavijest:

- Uređaj mora imati instaliran aplikaciju Portal tvrtke.  

- Uređaj mora dopustiti aplikaciji Portal tvrtke za slanje push obavijesti. Kada je aplikacija instalirana ili ažurirana, ona će zatražiti od korisnika da dopusti obavijesti.

- Android uređaji moraju imati instalirane usluge Google Play.

- Uređaj mora biti upisan s Intune.

Dodatne informacije, uključujući kako poslati poruku, potražite u [dokumentaciji značajke](https://docs.microsoft.com/intune/custom-notifications).
