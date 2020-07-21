---
title: Brisanje sirotišnog korisnika s lokalnog poslužitelja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197822"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Brisanje sirotišnog korisnika s lokalnog poslužitelja

Da biste uklonili napuštenog korisnika, slijedite ove korake:

1. Prisilno sinkronizacija direktorija slijedeći upute u odjeljku [Što je hibridni identitet servisa Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Da biste provjerili sinkronizaciju direktorija, pročitajte [što je hibridni identitet servisa Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Ako sinkronizacija ispravno funkcionira, ali brisanje objekta servisa Active Directory ne propagira Azure AD, ručno uklonite napušteni objekt pomoću jednog od sljedećih cmdleta Azure Active Directory Module za Windows PowerShell:

    Ukloni-MsolKontakt  
    Ukloni-MsolGroup  
    Ukloni-MsolUser

    Na primjer, da biste uklonili john.smith@contoso.com za napušteni korisnički ID, izvorno stvoren pomoću sinkronizacije direktorija, pokrenite cmdlet:

    Maknuti-MsolUser – UserPrincipalName John.Smith@Contoso.com