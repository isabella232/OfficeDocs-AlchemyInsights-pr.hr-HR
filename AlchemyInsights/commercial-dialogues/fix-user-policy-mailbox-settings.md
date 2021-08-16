---
title: Rješavanje problema s korisničkim pravilnikom/postavkama poštanskog sandučića
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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034710"
---
# <a name="fix-user-policymailbox-settings"></a>Rješavanje problema s korisničkim pravilnikom/postavkama poštanskog sandučića

Postavke bezvrijedne pošte u poštanskom sandučiću utjecale su na ovu poruku. Da biste pregledali postavke, učinite sljedeće:

1. Pokrenite Exchange Management Shell. Dodatne informacije potražite u članku [Otvaranje ljuske Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Pokrenite ovu naredbu (pomoću korisnikova adrese  **e-pošte): get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Provjerite je li adresa e-pošte pošiljatelja dio **trustedSendersAndDomains** ili **BlockedSendersAndDomains**. Ako se adresa e-pošte nalazi na jednom od popisa, možda ćete je morati ukloniti. Dodatne informacije potražite u članku [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
