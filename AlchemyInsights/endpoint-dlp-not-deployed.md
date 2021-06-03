---
title: DLP krajnje točke nije implementiran na korisnikov uređaj
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731320"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP krajnje točke nije implementiran na korisnikov uređaj

Ako postavka Sprječavanja gubitka podataka krajnje točke (DLP) nije primijenjena na korisnikov uređaj, provjerite ispunjavate li sljedeće preduvjete:

- Windows 10 x64 međuverzija 1809 ili novija instalirana je na uređaju.
- Instalirana je verzija klijenta za zaštitu od zlonamjernog softvera 4.18.2009.7 ili novija.
- Uređaj je **jedan od** ovih:
    
    - Azure Active Directory (Azure AD) pridruženo
    - Hibridno pridruženo azure AD
    - AAD registriran

- Da biste nametli akcije pravilnika, provjerite je li Chromium preglednik Microsoft Chromium Edge instaliran na krajnjem uređaju.

Dodatne preduvjete za implementaciju DLP-a krajnje točke pogledajte u članku [Početak rada s sprječavanjem gubitka podataka krajnje točke](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).