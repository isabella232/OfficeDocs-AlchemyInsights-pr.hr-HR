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
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086156"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Slanje prilagođenih obavijesti korisnicima upravljanih uređaja sa sustavom iOS i Android

Prilagođene obavijesti za Intune obrađuje aplikacija Company Portal na uređaju korisnika. Aplikacija zatim stvara push obavijest na tom uređaju.

U nastavku su preduvjeti uređaja za podršku primitku prilagođenih obavijesti, a da bi aplikacija potom stvorili push obavijest:

- Uređaj mora imati instaliranu Company Portal aplikaciju.  

- Uređaj mora omogućiti aplikaciji Company Portal slanje automatskih obavijesti. Kada je aplikacija instalirana ili ažurirana, od korisnika će se zatražiti da dopusti obavijesti.

- Na uređajima sa sustavom Android moraju biti instalirani servisi Google Play.

- Uređaj se mora registrirati uz Intune.

Dodatne informacije, uključujući slanje poruke, potražite u dokumentaciji [o značajkama](https://docs.microsoft.com/intune/custom-notifications).
