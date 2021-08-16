---
title: Kod pogreške 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ako vam se prilikom aktivacije sustava Office 2013 u implementacijama servisa udaljene radne površine (RDS) prikazuje pogreška, preporučujemo da omogućite ADAL uređivanjem registra.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100754"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Pogreška prilikom aktivacije Office 2013 na servisima udaljene radne površine

Ako vam se prilikom aktivacije sustava Office 2013 u implementacijama servisa udaljene radne površine (RDS) prikazuje pogreška, preporučujemo da omogućite ADAL uređivanjem registra.
  
|**Ključ registra**|**Vrsta**|**Vrijednost**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Dodatne informacije potražite u članku [Omogućivanje moderne provjere autentičnosti za Office 2013 na Windows uređajima](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL je po zadanom omogućen u Microsoft 365 Apps za velike tvrtke i Office 2016. Servisi udaljene radne površine (RDS) prethodno su se nazvali Servisi terminala.
  