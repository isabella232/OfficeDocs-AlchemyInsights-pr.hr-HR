---
title: Omogućivanje nadzora poštanskog sandučića
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703563"
---
# <a name="enable-mailbox-auditing"></a>Omogućivanje nadzora poštanskog sandučića

Da biste omogućili nadzor poštanskog sandučića za jednog korisnika ili cijelu organizaciju, sljedeći cmdleti moraju se pokrenuti iz ljuske udaljene energije:
  
 **Jedan korisnik**
  
Set-Mailbox -Identitet "Jane Dow" -AuditEnabled $true
  
 **Organizacije**
  
Get-Mailbox-ResultSize Neograničeno -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true
  
[uči više](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

