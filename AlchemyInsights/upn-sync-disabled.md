---
title: Onemogućeno je sinkronizaciju UPN-a
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749506"
---
# <a name="upn-sync-disabled"></a>Onemogućeno je sinkronizaciju UPN-a

Ako ste pokrenuli sinkronizaciju sa servisom Azure AD prije 30. ožujka 2016, pokrenite sljedeći cmdlet Azure AD PowerShell da biste omogućili UPN meki podudaranje samo za vašu tvrtku ili ustanovu:
  
 **Set-MsolDirSyncFeature-značajka Enablesoftmatchibirn-Enable $True**
  
UPN mekana podudarnost automatski se uključi za tvrtke ili ustanove koje su pokrenule sinkronizaciju sa servisom Azure AD na ili nakon 30. ožujka 2016.
  
Da biste saznali više o omogućivanju meke podudaranja na UPN-u i drugim značajkama sinkronizacije, pročitajte [značajke servisa Azure ad Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

