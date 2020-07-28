---
title: Nije moguće promijeniti Korisničko ime
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438887"
---
# <a name="unable-to-change-username"></a>Nije moguće promijeniti Korisničko ime

U nekim slučajevima promjene UPN (UserPrincipalName) nisu propagirane u oblak. Možda ćete primiti pogreške provjere valjanosti na portalu sustava Office 365 ili ne možete promijeniti korisničko ime ili adresu e-pošte. Da biste riješili taj problem, ručno postavite UserPrincipalName pomoću ove naredbe PowerShell.

**Primjer: Preimenovanje korisnika**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Ova naredba davidc@contoso.com preimenuje u davidchew@contoso.com.

Dodatne informacije potražite [u odjeljku Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).