---
title: Lokacija podataka
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207253"
---
# <a name="data-location"></a>Lokacija podataka

Mjesto vašeg Office 365 klijenta možete vidjeti u centru za administraciju ili povezivanjem s Exchange Online putem PowerShell.


**Centar za administraciju:**
1. Prijavite se u [centar za administraciju](https://admin.microsoft.com/Adminportal/Home).
2. Odaberite **Postavke** > **organizacije profil**.
3. U odjeljku **lokacija podataka**odaberite **Prikaz detalja**.


**Powershell:**
1. Povežite se s Exchangeovim internetom pomoću Windows PowerShell.
2. Izvršite cmdlet [Get-Organizatacionalunit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) da biste prikazali popis svojstava vašeg stanara. 
3. Pogledajte svojstvo OrganizationId.

Kada imate mjesto podataka za EXO i SPO, možete odrediti mjesto podataka za druge usluge koje možete koristiti na [mjestu gdje se nalaze vaši podaci](https://products.office.com/where-is-your-data-located).