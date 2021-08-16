---
title: AAD Povezivanje
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
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097298"
---
# <a name="notification-aad-connect"></a>AAD Povezivanje

- Provjerite jeste li ovlašteni za izvođenje operacije. Globalni administratori po zadanom imaju pristup. Uz to, pomoću kontrole pristupa [utemeljene na ulogama možete delegirati](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) dozvolu za registraciju suradniku.
- Provjerite jesu li obavezne krajnje točke omogućene, a ne blokirane zbog vatrozida. Detalje potražite u odjeljku [Preduvjeti](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registracija ne može uspjeti zbog odlazne komunikacije koja je podložan SSL pregledu mrežnog sloja.
- Provjerite jeste li potvrdili postavke obavijesti za Azure AD Povezivanje Stanje i pregledajte postavku. Upute za konfiguriranje postavki obavijesti za obavijesti za Azure AD Povezivanje obavijesti o stanju pogledajte u ovom [vodiču.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Dodatne informacije o izvješću o sinkronizaciji servisa AAD Povezivanje stanje i kako ga preuzeti potražite u članku [Izvješće o sinkronizaciji na razini objekta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Da biste otklonili poteškoće Povezivanje upozorenja o zdravlju, slijedite vodič za otklanjanje poteškoća za upozorenja o svježini podataka sustava [AAD Povezivanje](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Zdravlje i najčešća pitanja potražite u članku Najčešća pitanja o [instalaciji servisa AAD Povezivanje Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
