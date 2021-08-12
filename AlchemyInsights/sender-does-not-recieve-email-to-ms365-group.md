---
title: Pošiljatelj ne prima e-poštu poslanu Microsoft 365 grupi
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
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958289"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Pošiljatelj ne prima e-poštu poslanu Microsoft 365 grupi

Po zadanom pošiljatelj poruke e-pošte u grupu Microsoft 365 ne prima kopiju poruke u ulaznoj pošti, čak i ako je pošiljatelj član grupe.

Pomoću ove naredbe EXO PowerShell pošiljatelju omogućite primanje kopije svake poruke e-pošte koju pošalje grupi Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Da biste omogućili postavku za sve poštanske sandučiće odjednom:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Napomena** Za promjene te postavke potrebno je do sat vremena da bi stupjete na snagu.