---
title: Problem sa AAD Povezivanje Health
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923744"
---
# <a name="problem-with-aad-connect-health"></a>Problem sa AAD Povezivanje Health

- Provjerite jeste li ovlašteni za izvođenje operacije. Globalni administratori po zadanom imaju pristup. Uz to, pomoću kontrole pristupa [utemeljene na ulogama možete delegirati](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) dozvolu za registraciju suradniku.
- Provjerite jesu li obavezne krajnje točke omogućene, a ne blokirane zbog vatrozida. Detalje potražite u odjeljku [Preduvjeti](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registracija ne može uspjeti zbog odlazne komunikacije koja je podložan SSL pregledu mrežnog sloja.
- Provjerite jeste li potvrdili postavke obavijesti za Azure AD Povezivanje Stanje. Pregledajte postavku. Ovaj [vodič](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) može vam pomoći da shvatite kako konfigurirati postavke obavijesti za obavijesti za Azure AD Povezivanje obavijesti o stanju.
- Dodatne informacije o izvješću o sinkronizaciji servisa AAD Povezivanje stanje i kako ga preuzeti potražite u članku [Izvješće o sinkronizaciji na razini objekta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Da biste otklonili poteškoće s upozorenjima za AAD Povezivanje Zdravlje, slijedite vodič za otklanjanje poteškoća za upozorenja o svježini podataka o stanju sustava [AAD Povezivanje](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) i najčešća pitanja potražite u članku Najčešća pitanja o [instalaciji servisa AAD Povezivanje Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
