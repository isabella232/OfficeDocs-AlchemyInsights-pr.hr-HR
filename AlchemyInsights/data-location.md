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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655274"
---
# <a name="data-location"></a>Lokacija podataka

Lokaciju klijenta možete vidjeti u centru za administratore ili povezivanjem sa sustavom Exchange Online putem komponente PowerShell.


**Centar za administratore:**
1. Prijavite se u centar za [administratore](https://admin.microsoft.com/Adminportal/Home).
2. Odaberite**Profil organizacije** **postavki** > .
3. U **odjeljku Lokacija podataka**odaberite **Prikaz pojedinosti**.


**Powershell:**
1. Povežite se sa sustavom Exchange Online pomoću komponente Windows PowerShell.
2. Izvršite cmdlet [Get-OrganizationUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) da biste prikazali popis svojstava klijenta. 
3. Pogledaj vlasništvo OrganizationId.

Kada imate lokaciju podataka za EXO i SPO, možete odrediti lokaciju podataka za druge usluge koje možete koristiti iz [mjesta gdje se nalaze vaši podaci](https://products.office.com/where-is-your-data-located).