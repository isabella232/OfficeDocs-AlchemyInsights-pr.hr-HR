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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816340"
---
# <a name="create-a-group"></a>Stvaranje grupe

U ovoj se temi opisuje stvaranje grupe.

**Dozvola za stvaranje grupe**

Provjerite jeste li ovlašteni za stvaranje nove grupe. Globalni administratori mogu onemogućiti stvaranje grupe na portalu Azure ili ploči programa Access. Možda će vam biti potreban administrator da biste za vas stvorili novu grupu ili vam dali odgovarajuće dozvole.

**Upravljanje dozvolama za stvaranje grupe**

1. Globalni administratori mogu upravljati dozvolama za stvaranje grupa (iz sigurnosnih razloga) ili grupama sustava Office 365 stvorenima na portalu Azure ili na ploči programa Access, odabirom mogućnosti "Korisnici mogu stvarati sigurnosne grupe na portalima azure" ili "Korisnici mogu stvarati grupe sustava Office 365 na portalima azure" u odjeljku Sve **grupe**  >  **Općenito (Postavke).**
2. Ako imate licencu za Azure Active Directory P1 Premium, možete i ograničiti stvaranje grupe da biste odabrali grupu korisnika.

**Onemogućivanje obavijesti o dobrodošlici za nove članove grupe sustava Office 365**

Obavijest dobrodošlice poslana korisnicima koji su dodani u grupe sustava Office 365 može se onemogućiti postavljanjem **UnifiedGroupWelcomeMessageEnabled** na False u ljuski Powershell. Ovdje se informirajte o [ovoj postavki](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

