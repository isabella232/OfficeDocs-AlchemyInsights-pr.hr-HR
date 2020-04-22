---
title: Promjena zahtjeva za jaku lozinku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706553"
---
# <a name="change-strong-password-requirement"></a>Promjena zahtjeva za jaku lozinku

Microsoft prema zadanim postavkama zahtijeva jake lozinke. 

Koristeći PowerShell, možete onemogućiti jake lozinke za određene korisnike s ovom naredbom:<br>
*Zalazak-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired $false*

- [Dodatne informacije o pravilima za lozinku](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kako se povezati sa sustavom Microsoft 365 pomoću komponente PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Dodatne informacije o powershell msoluser naredbe](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
