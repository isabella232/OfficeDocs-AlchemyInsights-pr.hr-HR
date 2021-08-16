---
title: Dodjeljivanje grupa ulozi servisa Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036232"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Dodjeljivanje grupa ulozi servisa Azure AD

Da biste grupi Azure AD dodijelili izvor ovlasti na servisu Azure AD ulozi azure AD, učinite sljedeće:

1. Stvaranje nove grupe – da biste stvorili novu grupu:

    a. Prijavite se u centar za administratore servisa Azure AD s **ovlastima administratora uloga ili** **dozvola globalnog administratora.**
    b. Odaberite **Azure Active Directory > Grupe > Sve grupe > Nova grupa**.
    c. Stvorite grupu.

2. Dodijelite ulogu grupi tijekom stvaranja grupe ili nakon stvaranja grupe.

    a. Da biste grupi dodijelili ulogu u vrijeme stvaranja grupe, uključite preklopne uloge servisa **Azure AD** mogu se dodijeliti grupi i stvoriti grupu.
    b. Da biste grupi dodijelili ulogu nakon stvaranja, otvorite karticu Dodijeljene **uloge** za novostvorenu grupu i dodijelite je grupi.  

**Upravljanje članstvom u grupi dodijeljenoj ulozi platforme Azure AD**

Da bi se spriječilo povećanje ovlasti, samo administratori uloga s ovlastima i globalni administratori po zadanom mogu izmijeniti članstvo grupe dodijeljene ulozi. No mogu odabrati dodijeliti vlasnika za takvu grupu i delegirati taj zadatak.

Dodatne informacije o dodjeli grupa u oblaku ulogama servisa Azure AD potražite u članku [Dodjela uloga za AD grupi u oblaku](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Dodatne informacije o ulogama za otklanjanje poteškoća dodijeljenim grupama u oblaku potražite u članku Otklanjanje [poteškoća s ulogama dodijeljenima grupama u oblaku](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





