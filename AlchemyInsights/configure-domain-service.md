---
title: Konfiguriranje servisa domene
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884864"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Nemogućnost omogućivanja AAD-DS ili implementacija ne uspijeva

Da biste riješili problem servisa Azure AD Domain (AAD-DS) koji nije omogućen ili se nije uspio implementirati, slijedite sljedeće korake:

1. Ako koristite već postojeću virtualnu mrežu, provjerite je li NSG za pravila koja blokiraju priključke potrebne za sinkronizaciju u AAD-DS-u na portalu https://aka.ms/aadds-networking .
2. Provjerite je li poruka o pogrešci odgovorena u ovom vodiču za otklanjanje poteškoća koji je dostupan u programu  https://aka.ms/aadds-troubleshoot-enable .
3. Isprobajte implementaciju servisa Azure AD domene u novoj virtualnoj mreži.
4. Slijedite vodič za početak rada na načinu implementacije AAD-DS- [a: stvaranje i konfiguriranje servisa za domenu programa AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Ako imate problema s implementacijom servisa Azure AD domena, pročitajte članak [Otklanjanje poteškoća s domenskim servisima Azure ad](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) da biste riješili česte pogreške da bi vam pomoglo da ponovno pokrenete rad. 

**Nije moguće onemogućiti AAD-DS**

AAD-DS nije moguće pauzirati. Ako želite prestati koristiti upravljane domene, ona se mora izbrisati.
Da biste izbrisali upravljanu domenu, pročitajte članak [Brisanje servisa za domenu AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



