---
title: Problem s povezivanjem servisa AAD za zdravlje
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481152"
---
# <a name="problem-with-aad-connect-health"></a>Problem s povezivanjem servisa AAD za zdravlje

- Provjerite jeste li ovlašteni za izvršavanje operacije. Globalni administratori imaju pristup prema zadanim postavkama. Uz to, pomoću [kontrole pristupa temeljene na ulogama](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) možete delegirati dozvolu za registraciju suradnika.
- Provjerite jesu li obavezne krajnje točke omogućene i nije li blokirana zbog vatrozida. Pojedinosti potražite u članku [Preduvjeti](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registracija može propasti zbog odlazne komunikacije koja je izložena SSL inspekciji putem mrežnog sloja.
- Provjerite jeste li potvrdili postavke obavijesti o zdravlju za Azure AD Connect. Pregledajte postavku. Ovaj [vodič](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) može vam pomoći da razumijete kako konfigurirati postavke obavijesti za obavijesti o zdravlju servisa Azure ad Connect.
- Da biste saznali više o izvješću o sinkronizaciji programa AAD Connect i kako ga preuzeti, pročitajte članak [izvješće o sinkronizaciji razina objekta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Da biste otklonili poteškoće s aplikacijom AAD Connect zdravstvene obavijesti, slijedite [upute za otklanjanje poteškoća za AAD povežite upozorenja o svježini podataka](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) i najčešća pitanja, pročitajte članak [zajednički AAD Connect pitanja o zdravstvenoj instalaciji](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
