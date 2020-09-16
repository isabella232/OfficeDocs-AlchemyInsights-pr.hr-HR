---
title: Pogreška za ispravljanje 0x8004de40 na servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745122"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Pogreška za ispravljanje 0x8004de40 na servisu OneDrive

Ako vam se prikaže pogreška 0x8004de40 sa servisom OneDrive:

- Ponovno pokrenite računalo koje je utjecalo na nju dok ste povezani s domenom tvrtke Acitve.
- Ako ponovno pokretanje ne riješi problem, poništite pridruživanje i ponovno se pridruži uređaju iz servisa Azure AD. 

**Imajte**na glavi: prilikom izvođenja ovih koraka trebali biste biti na mreži korporativnih tvrtki. Ne izvodite ove korake kada se ne možete povezati s korporacijskom infrastrukturom (na primjer, tijekom putovanja). 

- Otvaranje povišenog naredbenog upita. 
- Da biste otvorili povišeni naredbeni upit, kliknite- **Start**, desnom tipkom miša kliknite **naredbeni upit**, a zatim kliknite **Pokreni kao administrator**.
- Upišite *dsregcmd/ostavite* i pritisnite **Enter**.
- Kada završite, upišite *dsregcmd/Join* i pritisnite **Enter**.
- Kada završite, zatvaranje naredbenog upita.
- Ponovno pokrenite računalo i prijavite se na OneDrive.