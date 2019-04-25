---
title: Kod pogreške 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ako si primanje pogreške tijekom aktivacije Office 2013 na uvođenja usluge udaljene radne površine (ZAPISI), razmislite o omogućavanju ADAL uređivanjem registra.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402731"
---
Ako si primanje pogreške tijekom aktivacije Office 2013 na uvođenja usluge udaljene radne površine (ZAPISI), razmislite o omogućavanju ADAL uređivanjem registra. 
  
|**Ključ registra**|**Vrsta**|**Vrijednost**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Dodatne informacije potražite [Omogućiti Moderna provjere autentičnosti 2013 Office na Windows uređajima](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL je po zadanom omogućen u Office 365 ProPlus i 2016 za Office. > usluge udaljene radne površine (ZAPISI) je prethodno pod nazivom servisa Terminal Services. 
  

