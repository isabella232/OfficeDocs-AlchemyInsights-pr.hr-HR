---
title: Kontroler domene
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900800"
---
# <a name="domain-controller"></a>Kontroler domene

**Nemogućnost omogućivanja AAD-DS ili implementacija ne uspijeva**

Da biste riješili problem servisa Azure AD Domain (AAD-DS) koji nije omogućen ili se nije uspio implementirati, slijedite sljedeće korake:

1. Ako koristite već postojeću virtualnu mrežu, provjerite je li NSG za pravila koja blokiraju priključke potrebne za sinkronizaciju u AAD-DS-u na portalu https://aka.ms/aadds-networking .
2. Provjerite je li poruka o pogrešci odgovorena u ovom vodiču za otklanjanje poteškoća koji je dostupan u programu  https://aka.ms/aadds-troubleshoot-enable .
3. Isprobajte implementaciju servisa Azure AD domene u novoj virtualnoj mreži.
4. Slijedite vodič za početak rada na načinu implementacije AAD-DS-a, koji je dostupan na [vodiču za stvaranje servisa Azure ad domene](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Ako imate problema s implementacijom servisa Azure AD domena, pročitajte članak [Otklanjanje poteškoća s domenskim servisima Azure ad](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) da biste riješili česte pogreške da bi vam pomoglo da ponovno pokrenete rad. 

**Nije moguće onemogućiti AAD-DS**

AAD-DS nije moguće pauzirati. Ako želite prestati koristiti upravljane domene, ona se mora izbrisati.

Ako ste naletjeli na probleme, da biste riješili česte poruke o pogreškama i povezali upute za otklanjanje poteškoća koje će vam pomoći da ponovno pokrenete pokretanje, pročitajte članak [Otklanjanje poteškoća s domenama servisa Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
