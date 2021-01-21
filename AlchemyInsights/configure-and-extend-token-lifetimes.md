---
title: Konfiguriranje i proširivanje životnog razdoblja tokena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916687"
---
# <a name="configure-and-extend-token-lifetimes"></a>Konfiguriranje i proširivanje životnog razdoblja tokena

Možete navesti vijek trajanja programa Access, SAML ili ID token koji je izdala Microsoftova osobna platforma. U svim aplikacijama u vašoj tvrtki ili ustanovi možete postaviti znak trajanja tokena, za višečlansku (multi-organizacijsku) aplikaciju ili za određenog upravitelja servisa u vašoj tvrtki ili ustanovi. Dodatne informacije potražite u odjeljku [simbol](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

Primjeri, pročitajte [primjere kako konfigurirati životni vijek tokena](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Upute za konfiguriranje životnog vijeka i kompatibilnosti tokena u servisu Azure Active Directory B2C (Azure AD B2C) potražite [u članku Konfiguriranje žetona u servisu Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

U članku [Konfiguriranje ponašanja sesije u servisu Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) opisuje metode jedinstvenog prijave (SSO) koje se koriste u servisu Azure ad B2C i olakšava odabir NAJPRIKLADNIJE metode SSO prilikom konfiguriranja pravilnika.

**Koliko dugo traje tokeni? Koliko dugo vrijede?**

Životni vijek tokena je 1 sat, a Trajanje sesije 24 sata. To znači da ako u 24 sata ne bude nikakvih zahtjeva, morat ćete se ponovno prijaviti prije nego što zatražite novi token.

> [!NOTE]
> Nakon 30 svibnja 2020, nijedan novi stanar neće moći koristiti pravilnik o životnom vijeku tokena za konfiguriranje sesija i osvježavanja žetona. Ukidanje će se dogoditi u roku od nekoliko mjeseci nakon toga, što znači da ćemo prekinuti s poštivanju postojećih sesija i osvježavanjem znakova tokena. Još uvijek možete konfigurirati Access token za životni vijek nakon razdiobe.






