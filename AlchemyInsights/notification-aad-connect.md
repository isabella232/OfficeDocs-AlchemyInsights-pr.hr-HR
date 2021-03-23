---
title: Prijavljivanje AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035088"
---
# <a name="notification-aad-connect"></a>Prijavljivanje AAD Connect

- Provjerite jeste li ovlašteni za izvršavanje operacije. Globalni administratori imaju pristup prema zadanim postavkama. Uz to, pomoću [kontrole pristupa temeljene na ulogama](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) možete delegirati dozvolu za registraciju suradnika.
- Provjerite jesu li obavezne krajnje točke omogućene i nije li blokirana zbog vatrozida. Pojedinosti potražite u članku [Preduvjeti](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registracija može propasti zbog odlazne komunikacije koja je izložena SSL inspekciji putem mrežnog sloja.
- Provjerite jeste li potvrdili postavke obavijesti za Azure AD Connect zdravlje i pregledajte postavke. Da biste razumjeli kako konfigurirati postavke obavijesti za obavijesti o zdravlju u servisu Azure AD Connect, pogledajte ovaj [vodič](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Da biste saznali više o izvješću o sinkronizaciji programa AAD Connect i kako ga preuzeti, pročitajte članak [izvješće o sinkronizaciji razina objekta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Da biste otklonili poteškoće s upozorenjima za AAD Connect, slijedite [upute za otklanjanje poteškoća za AAD povežite upozorenja o osvježenosti podataka](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) i najčešća pitanja, pročitajte članak [zajednički AAD Connect pitanja o zdravstvenoj instalaciji](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
