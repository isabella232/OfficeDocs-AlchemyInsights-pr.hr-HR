---
title: Šifra pogreške 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ako se prilikom aktivacije sustava Office 2013 na implementacijama servisa udaljene radne površine (RDS) pojavljuje pogreška, razmislite o omogućivanju ADAL-a uređivanjem registra.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703130"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Pogreška prilikom aktivacije sustava Office 2013 na servisima udaljene radne površine

Ako se prilikom aktivacije sustava Office 2013 na implementacijama servisa udaljene radne površine (RDS) pojavljuje pogreška, razmislite o omogućivanju ADAL-a uređivanjem registra.
  
|**Ključ registra**|**Tip**|**Vrijednost**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Dodatne informacije potražite u [odjeljku Omogućivanje moderne provjere autentičnosti za Office 2013 na uređajima sa sustavom Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL je omogućen prema zadanim postavkama u Aplikacijama microsoft 365 za tvrtke i Office 2016. Servisi udaljene radne površine (RDS) prethodno su bili nazvani Servisi terminala.
  