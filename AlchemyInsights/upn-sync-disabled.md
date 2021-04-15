---
title: UPN sinkronizacija je onemogućena
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782143"
---
# <a name="upn-sync-disabled"></a>UPN sinkronizacija je onemogućena

Ako ste počeli sinkronizirati sa servisom Azure AD prije 30. ožujka 2016., pokrenite sljedeći cmdlet komponente Azure AD PowerShell da biste omogućili UPN meko podudaranje samo za svoju organizaciju:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN meko podudaranje automatski se uključuje za tvrtke ili ustanove koje su se počele sinkronizirati sa servisom Azure AD ili nakon 30. ožujka 2016.
  
Dodatne informacije o omogućivanju mekog podudaranja na UPN-u i drugim značajkama sinkronizacije potražite u članku Značajke servisa za sinkronizaciju [servisa Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

