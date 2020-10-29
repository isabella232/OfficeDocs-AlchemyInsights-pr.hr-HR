---
title: Otklanjanje poteškoća s programom Microsoft Defender za Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801435"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Otklanjanje poteškoća s programom Microsoft Defender za Office 365

- Primjećujete li kašnjenje u isporuci poruke? Pomoću mogućnosti [dinamičke isporuke](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) u pravilima programa ATP siguran privici. Time će se izbjeći kašnjenje poruka dok se primatelji štite od zlonamjernih datoteka.

- Želite li Microsoftu prijaviti netočne ili FALSE negative? Upotrijebite ovu [vezu](https://www.microsoft.com/wdsi/filesubmission/) da biste poslali datoteke za analizu.

- Jeste li znali da možete omogućiti sigurnu vezu za zaštitu interne e-pošte poslane među primateljima unutar tvrtke ili ustanove? Slijedite ove korake:

  1. Idite na [https://protection.office.com](https://protection.office.com) i prijavite se pomoću računa globalnog administratora ili sigurnosnog administratora.

  2. U lijevoj navigacijskom oknu u odjeljku **Upravljanje prijetnjama** odaberite **Policy** \> **sigurne veze** za pravilnik.

  3. U **pravilima koja se odnose na cijelu tvrtku ili ustanovu** odaberite pravilo, a zatim kliknite **Uredi** .

  4. U odjeljku **Postavke** omogućite **primjenu sigurnih veza na poruke poslane unutar tvrtke ili ustanove** .
