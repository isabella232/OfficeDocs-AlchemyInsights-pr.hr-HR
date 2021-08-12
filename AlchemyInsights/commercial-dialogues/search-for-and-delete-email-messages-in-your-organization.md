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
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948875"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi

Slijedite ove korake:

1. Ako niste globalni administrator, da biste potražili poruke, vaš račun mora biti dodan u grupu **uloga upravitelja elektroničkih** elektroničkih obveza ili ulogu za upravljanje **pretraživanjem usklađenosti.** Da biste izbrisali poruke, morate se pridružiti grupi uloga **za upravljanje organizacijom** ili ulozi upravljanja pretraživanjem **i čišćenjem.** Dozvole za te uloge dodjeljuju se u centru [za & usklađenosti.](https://protection.office.com)
2. [Stvorite pretraživanje sadržaja da](https://docs.microsoft.com/office365/securitycompliance/content-search) biste pronašli poruku koju želite izbrisati.
3. [Povezivanje na powershell centra za & sigurnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Ako koristite MFA, pročitajte sljedeće upute: Povezivanje [za sigurnost & komponente PowerShell pomoću višestruke provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Izbrišite poruku: pokrenite `New-ComplianceSearchAction` cmdlet da biste izbrisali poruku. Izbrisane se poruke premještaju u korisnikov mapu Stavke koje se mogu oporaviti. Primjer naredbe pogledajte u [3. koraku: brisanje poruke.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
