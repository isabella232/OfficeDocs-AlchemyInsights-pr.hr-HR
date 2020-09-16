---
title: Pošiljatelj ne prima e-poštu poslanu u grupu Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751307"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Pošiljatelj ne prima e-poštu poslanu u grupu Microsoft 365

Pošiljatelj poruke e-pošte prema zadanim postavkama u grupi Microsoft 365 ne prima kopiju poruke u ulaznoj pošti, čak i ako je pošiljatelj član grupe.

Upotrijebite ovu naredbu EXO PowerShell da biste pošiljatelju dopustili primanje kopije svake poruke e-pošte koju pošalju u grupu Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Da biste istodobno omogućili postavku za sve poštanske sandučiće:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Notes** Promjene ove postavke uzimaju učinak na jedan sat.