---
title: Poruke poslane u grupu okruženja Microsoft 365 ne primaju svi članovi
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976497"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Poruke poslane u grupu okruženja Microsoft 365 ne primaju svi članovi

Pobrinite se da se svi članovi grupe pretplate na primanje poruka e-pošte. Pogledajte [Praćenje grupe u programu Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Da biste provjerili status poruka članova koji su se pretplatili na poruke e-pošte grupe, pokrenite sljedeću naredbu u sustavu [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Koristite se sljedećom naredbom sustava EXO PowerShell da biste konfigurirali da svi članovi grupe u svoju mapu ulazne pošte primaju poruke e-pošte poslane u grupu okruženja Microsoft 365:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Na primjer:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`