---
title: Brisanje korisnika koji su napušteni s lokalnog poslužitelja
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
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680127"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Brisanje korisnika koji su napušteni s lokalnog poslužitelja

Da biste uklonili siroog korisnika, slijedite ove korake:

1. Prisilno Sinkroniziranje direktorija slijedite upute u odjeljku [što je hibridni identitet sa servisom Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Da biste potvrdili sinkronizaciju direktorija, pročitajte članak [što je hibridni identitet sa servisom Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Ako sinkronizira funkcionira ispravno, no Brisanje objekta servisa Active Directory ne prenosi se na Azure AD, ručno uklonite napušteni objekt pomoću jednog od sljedećih modula za Azure Active Directory za Windows PowerShell za cmdlete:

    Uklanjanje-MsolContact  
    Uklanjanje-MsolGroup  
    Uklanjanje-MsolUser

    Da biste, primjerice, uklonili john.smith@contoso.com ID korisnika, izvorno stvoren pomoću sinkronizacije direktorija, pokrenite cmdlet:

    Uklanjanje-MsolUser – UserPrincipalName John.Smith@Contoso.com