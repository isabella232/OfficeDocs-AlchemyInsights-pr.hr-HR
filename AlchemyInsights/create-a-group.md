---
title: Stvaranje grupe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929297"
---
# <a name="create-a-group"></a>Stvaranje grupe

U ovoj se temi opisuje stvaranje grupe.

**Dozvola za stvaranje grupe**

Provjerite jeste li ovlašteni za stvaranje nove grupe. Globalni administratori mogu onemogućiti stvaranje grupe na portalu Azure ili ploči programa Access. Možda će vam biti potreban administrator da biste za vas stvorili novu grupu ili vam dali odgovarajuće dozvole.

**Upravljanje dozvolama za stvaranje grupe**

1. Globalni administratori mogu upravljati dozvolama za stvaranje grupa (iz sigurnosnih razloga) ili grupama sustava Office 365 stvorenima na portalu Azure ili ploči programa Access tako da u odjeljku Sve grupe Općenito (Postavke) odaberete "Korisnici mogu stvarati sigurnosne grupe" ili "Korisnici mogu stvarati grupe sustava Office 365 na portalima  >  **azure".**
2. Stvaranje grupe možete ograničiti i tako da odaberete grupu korisnika ako imate licencu za Azure Active Directory P1 premium grupe.

**Onemogućivanje obavijesti o dobroj dobrodošlici za nove Office 365 članove grupe**

Obavijest dobrodošlice poslana korisnicima koji su dodani u Office 365 može se onemogućiti postavljanjem **UnifiedGroupWelcomeMessageEnabled** na False u ljuski Powershell. Ovdje se informirajte o [ovoj postavki](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

