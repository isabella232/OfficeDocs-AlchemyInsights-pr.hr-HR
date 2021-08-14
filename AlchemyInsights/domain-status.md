---
title: Status domene – nije odabran nijedan servis
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 1ddf6475e7cf466a39f76486e0f809097917657bc8f4ae7f7f2b516657308f39
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947435"
---
# <a name="domain-status---no-services-selected"></a>Status domene – nije odabran nijedan servis

**Nijedan odabrani servis** ne znači da niste odabrali servise Microsoft 365 kao što su Exchange Online, Skype za tvrtke ili Intune i Upravljanje mobilnim uređajima za Microsoft 365 za korištenje s prilagođenom domenom. Ako koristite hibridnu Exchange (Exchange lokalno uz Exchange Online) ili vanjsko filtriranje neželjene pošte uz Exchange i nijedan drugi Microsoft services, možete zanemariti tu poruku. Stanje domene dostupno je samo za domene koje su izravno povezane sa servisom.

Da biste odabrali servise za svoju domenu:

1. Na **Postavke** domene potvrdite okvir pokraj domene s porukom o  >  [](https://admin.microsoft.com/Adminportal/Home)statusu Nema **odabranih servisa**.
1. Odaberite **Upravljanje DNS-om** da biste pokrenuli čarobnjak za postavljanje domene.
    - Ako odaberete Dodaj **vlastite DNS zapise**, obavezno odaberite servis kada se to od vas zatraži. Dodatne usluge mogu biti dostupne u **odjeljku Dodatne mogućnosti**.
    - Ako odaberete Dopusti **Microsoftu dodavanje DNS** zapisa ili Dodatne mogućnosti Postavljanje mrežnih servisa za   >  **mene,** predloženi su i automatski odabrani svi dostupni servisi.
1. Nastavite kroz čarobnjak da biste dovršili postavljanje DNS-a i mogućnosti servisa.
 
Dodatnu pomoć za postavljanje domene pogledajte u članku Dodavanje DNS zapisa radi [povezivanja domene](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

