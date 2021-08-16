---
title: Priprema za upotrebu protokola TLS 1.2 u okruženju Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 79a9dc3833f8329adeb24d27014d08c14eb93d1f5f840c5cfa2ce10991107b1c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040390"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Priprema za upotrebu protokola TLS 1.2 u okruženju Microsoft 365

Od 31. listopada 2018. Microsoft 365 nastavit će s prijelazom na TLS 1.2. Od 15. listopada 2020., O365 će početi ukidanje TLS 1.0 i 1.1 u cijelom servisu. Uvođenje te promjene nastavit će se tijekom sljedećih nekoliko tjedana i mjeseci, no korisnici ne bi trebali preuzimati pozive TLS 1.0/1.1 kada se angažiraju s O365 počevši od 15. listopada 2020. Kao što je prethodno priopćano (MC126199 u prosincu 2017., MC128929 u veljači 2018., MC186827 u srpnju 2019. i MC218794 u srpnju 2020.), sve naše internetske servise premještamo u sigurnost sloja transporta (TLS) 1,2+ da bismo pružili najbolje šifriranje u klasi te da bismo bili sigurniji. Korisnici i dalje mogu odabrati da TLS 1.0/1.1 na svojim poslužiteljima i resursima, ali pretpostavljaju da će samo TLS 1.2 ili noviji funkcionirati prilikom interakcije s resursima sustava O365.
  
Dodatne informacije o tim promjenama potražite ovdje [i](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) [ovdje.](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)

  