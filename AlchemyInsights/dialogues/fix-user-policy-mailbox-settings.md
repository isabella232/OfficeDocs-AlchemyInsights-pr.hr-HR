---
title: Rješavanje postavki korisničkog pravilnika/poštanskog sandučića
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692831"
---
# <a name="fix-user-policymailbox-settings"></a>Rješavanje postavki korisničkog pravilnika/poštanskog sandučića

Postavke bezvrijedne pošte na poštanskom sandučiću utječu na ovu poruku. Da biste pregledali postavke, učinite sljedeće:

1. Pokreni ljusku za upravljanje sustavom Exchange. Dodatne informacije potražite u članku [Otvaranje ljuske za upravljanje sustavom Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Pokretanje ove naredbe (pomoću adrese e-pošte korisnika):  **Nabavite-mailboxjunkmailconfiguration – Identity "user@domain.com"**
3. Provjerite je li adresa e-pošte pošiljatelja dio servisa **trustedesendersanddomains** ili **blockedsendersanddomains**. Ako je adresa e-pošte na jednom od popisa, možda ćete je morati ukloniti. Dodatne informacije potražite u članku [Konfiguracija postavke MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
