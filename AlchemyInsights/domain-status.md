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
ms.openlocfilehash: 1476a88c7b974a9e6cfe443f6842df8cdc3d7073a73c0add7e6f183dd0528de1
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57874387"
---
# <a name="domain-status---no-services-selected"></a>Status domene – nije odabran nijedan servis

**Nijedan odabrani servis** ne znači da niste odabrali nijedan servis Microsoft 365 kao što su Exchange Online, Skype za tvrtke ili Intune te Upravljanje mobilnim uređajima za Microsoft 365 za korištenje s prilagođenom domenom. Ako koristite hibridnu Exchange (Exchange lokalno uz Exchange Online) ili vanjsko filtriranje neželjene pošte s Exchange i bez Microsoft services, možete zanemariti tu poruku. Stanje domene dostupno je samo za domene koje su izravno povezane sa servisom.

Da biste odabrali servise za svoju domenu, odaberite sljedeće:

1. U **Postavke** Domena potvrdite okvir pokraj domene s porukom o  >  [](https://admin.microsoft.com/Adminportal/Home)statusu Nema **odabranih servisa**.
1. Odaberite **Upravljanje DNS-om** da biste pokrenuli čarobnjak za postavljanje domene.
    - Ako odaberete Dodaj **vlastite DNS zapise**, obavezno odaberite servis kada se to od vas zatraži. Dodatne usluge mogu biti dostupne u **odjeljku Dodatne mogućnosti**.
    - Ako odaberete Dopusti **Microsoftu dodavanje DNS** zapisa ili Dodatne mogućnosti Postavljanje mrežnih servisa za   >  **mene,** predloženi su i automatski odabrani svi dostupni servisi.
1. Nastavite kroz čarobnjak da biste dovršili postavljanje DNS-a i mogućnosti servisa.
 
Dodatnu pomoć za postavljanje domene pogledajte u članku Dodavanje DNS zapisa radi [povezivanja domene](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

