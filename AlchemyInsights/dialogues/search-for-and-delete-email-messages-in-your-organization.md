---
title: Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523382"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi

Slijedite ove korake:

1. Ako niste globalni administrator, da biste potražili poruke, vaš račun mora biti dodan u **grupu uloga menadžera za istraživanje** ili za **Upravljanje usklađivanjem pretraživanja**. Da biste izbrisali poruke, morat ćete se pridružiti **grupi uloga za upravljanje organizacijom** ili **ulogu pretraživanja i brisanja**. Dozvole za te uloge dodijeljene su u [centru za sigurnost & usklađenosti.](https://protection.office.com)
2. [Stvorite pretraživanje sadržaja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku koja će se izbrisati.
3. [Spojite se na sigurnosnu & PowerShell centra za usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Ako koristite MFA, pogledajte ove upute: [Povezivanje s pomoću komponente Security & u centru za usklađenost s višestrukim čimbenikom provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Izbrišite poruku: Pokrenite `New-ComplianceSearchAction` cmdlet da biste izbrisali poruku. Izbrisane poruke premještaju se u korisničku mapu stavke koje se mogu oporaviti. Naredba primjer potražite u odjeljku [treći korak: brisanje poruke.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
