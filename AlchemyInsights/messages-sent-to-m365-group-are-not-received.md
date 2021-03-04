---
title: Poruke poslane u grupu okruženja Microsoft 365 ne primaju svi članovi
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 39a4f8115a4742947b3e6394396be5ce3b01e772
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430675"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Poruke poslane u grupu okruženja Microsoft 365 ne primaju svi članovi

Provjerite jesu li se svi članovi grupe pretplatili na primanje poruka e-pošte. Pogledajte [Praćenje grupe u programu Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Da biste provjerili status poruka članova koji su se pretplatili na poruke e-pošte grupe, pokrenite sljedeću naredbu u sustavu [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Koristite se sljedećom naredbom sustava EXO PowerShell da biste konfigurirali da svi članovi grupe u svoju mapu ulazne pošte primaju poruke e-pošte poslane u grupu okruženja Microsoft 365:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`