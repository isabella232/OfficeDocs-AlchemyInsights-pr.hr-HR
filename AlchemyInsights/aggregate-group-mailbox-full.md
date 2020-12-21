---
title: Agregata grupnih poštanskih sandučića pun NDR primljenih za e-poštu poslanu u Microsoft 365 Group
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721783"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Agregata grupnih poštanskih sandučića pun NDR primljenih za e-poštu poslanu u Microsoft 365 Group

Da biste stvorili pravilo prijenosa sustava Exchange da biste tihi ispuštanje poruka e-pošte poslane u kumulativni poštanski sandučić, poslužite se sljedećim naredbenim eko-om

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Zamijenite SMTP adresu u **-SentTo** s SMTP adresom skupnog poštanskog sandučića grupe u vašem zakupcu. Možete dobiti SMTP adresu skupnog poštanskog sandučića grupe iz primljene NDR-a.



