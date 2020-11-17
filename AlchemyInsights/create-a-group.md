---
title: Stvaranje grupe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088576"
---
# <a name="create-a-group"></a>Stvaranje grupe

U ovoj se temi opisuje stvaranje grupe.

**Dozvola za stvaranje grupe**

Provjerite jeste li ovlašteni za stvaranje nove grupe. Globalni administratori mogu onemogućiti stvaranje grupe na portalu Azure ili na ploči programa Access. Da biste stvorili novu grupu za vas, možda će vam trebati administrator ili vam dati odgovarajuće dozvole.

**Upravljanje dozvolama za stvaranje grupa**

1. Globalni administratori mogu upravljati dozvolama za stvaranje grupe (zbog sigurnosnih razloga) ili grupa sustava Office 365 stvorenih na portalu Azure ili na ploči programa Access, odabirom mogućnosti "korisnici mogu stvarati sigurnosne grupe na servisu Azure portali" ili "korisnici mogu stvarati grupe sustava Office 365 u sustavima Azure portali" u **svim**  >  **općim grupama (postavke)**.
2. Možete i ograničiti Stvaranje grupe da biste odabrali grupu korisnika ako imate licencu za Azure Active Directory P1 Premium.

**Onemogućivanje obavijesti dobrodošlice za nove članove grupe sustava Office 365**

Obavijest dobrodošlice koja se šalje korisnicima koji su dodani u grupe sustava Office 365 može se onemogućiti postavljanjem **Unifiedgroupwelcomemessageenabled** u FALSE u komponenti PowerShell. Saznajte više o ovoj [postavci](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

