---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764253"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Rad s powershell ili skripte unutar Sharepoint Online? Posjetite linkove ispod za više informacija.
- [Početak rada s ljuskom za upravljanje sustavom SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Povezivanje sa SPO PowerShell s višestrukom provjerom autentičnosti (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint obrasci i postupci (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sadrži biblioteku naredbi komponente PowerShell koja vam omogućuje izvođenje složenih akcija upravljanja prema SPO-u.

> [!NOTE]
> - Ako imate problema s povezivanjem s ljuskom za upravljanje SPO-om, provjerite jeste li ažurirali najnoviju verziju i pokušajte [ponovno uvesti modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) pomoću *značajke "Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Ako pokušavate pokrenuti skripte modela objekta na strani klijenta, morat ćete imati instaliran [SDK za komponente klijenta sustava SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) na lokalnom računalu.
> - Ako imate problema s pokretanjem skripti iz komponente PowerShell, preporučujemo da pokrenete PowerShell kao administrator i promijenite [pravila izvršavanja](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).