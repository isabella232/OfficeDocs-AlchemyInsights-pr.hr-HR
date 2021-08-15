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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038104"
---
# <a name="upn-sync-disabled"></a>UPN sinkronizacija je onemogućena

Ako ste počeli sinkronizirati sa servisom Azure AD prije 30. ožujka 2016., pokrenite sljedeći cmdlet komponente Azure AD PowerShell da biste omogućili UPN meko podudaranje samo za svoju organizaciju:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN meko podudaranje automatski se uključuje za tvrtke ili ustanove koje su se počele sinkronizirati sa servisom Azure AD ili nakon 30. ožujka 2016.
  
Dodatne informacije o omogućivanju mekog podudaranja u sustavu UPN i drugim značajkama sinkronizacije potražite u članku [Značajke servisa za sinkronizaciju servisa Azure AD Povezivanje .](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

