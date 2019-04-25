---
title: Omogući nadzor poštanskog sandučića
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403739"
---
# <a name="enable-mailbox-auditing"></a>Omogući nadzor poštanskog sandučića

Da biste omogućili nadzor poštanskog sandučića za jednog korisnika ili cijeloj organizaciji sljedeće Cmdletovi morate pokrenuti iz Remote Shell uštede energije:
  
 **Jedan korisnik**
  
Skup-poštanski sandučić - identitet "Dow Ane" - AuditEnabled $true
  
 **Organizacija**
  
Dohvati poštanski sandučić - ResultSize neograničen - filtriranje {RecipientTypeDetails - eq "UserMailbox"} | Skup poštanski sandučić - AuditEnabled $true
  
[uči više](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

