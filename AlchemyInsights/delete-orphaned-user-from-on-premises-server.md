---
title: Brisanje napuštenog korisnika s lokalnog poslužitelja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: a6af617fa4235868f0754ff4c06f4cc73b1700ef14ea449dd1886ab100ddd384
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102235"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Brisanje napuštenog korisnika s lokalnog poslužitelja

Da biste uklonili napuštenog korisnika, slijedite ove korake:

1. Prisilno sinkroniziranje direktorija slijedeći upute u nastavku [Što je hibridni identitet Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Da biste provjerili sinkronizaciju direktorija, [pogledajte što je hibridni identitet Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Ako se funkcije sinkronizacije pravilno sinkroniziraju, ali brisanje objekta servisa Active Directory ne propagira na Azure AD, ručno uklonite napušteni objekt pomoću jednog od sljedećih Azure Active Directory modula za Windows PowerShell cmdlete:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Da biste, primjerice, uklonili napušteni korisnički ID john.smith@contoso.com, izvorno stvoren pomoću sinkronizacije direktorija, pokrenite cmdlet:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com