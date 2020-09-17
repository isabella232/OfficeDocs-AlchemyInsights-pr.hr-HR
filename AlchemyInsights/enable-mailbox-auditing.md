---
title: Omogućivanje nadzora poštanskog sandučića
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806283"
---
# <a name="enable-mailbox-auditing"></a>Omogućivanje nadzora poštanskog sandučića

Da biste omogućili nadziranje poštanskog sandučića za jednog korisnika ili cijelu tvrtku ili ustanovu, sljedeći se cmdleti moraju pokrenuti iz udaljenog dodatka Power Shell:
  
 **Jedan korisnik**
  
Zalazak-poštanski sandučić – identitet "Jane Dow"-AuditEnabled $true
  
 **Tvrtke ili ustanove**
  
Nabavite-Mailbox-rezultat neograničeno-filtar {RecipientTypeDetails-aq "UserMailbox"} | $true s mogućnošću postavljanje poštanskog sandučića
  
[uči više](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

