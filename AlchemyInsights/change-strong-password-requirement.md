---
title: Promjena preduvjeta neprobojnu lozinku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35701576"
---
# <a name="change-strong-password-requirement"></a>Promjena preduvjeta neprobojnu lozinku

Neprobojne lozinke potrebne su po zadanom. 

Koristite PowerShell možete onemogućiti neprobojne lozinke za određene korisnike s ovu naredbu:<br>
*Skup MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [Dodatne informacije o pravila lozinki](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kako povezati s O365 s PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Dodatne informacije o naredbe PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)