---
title: Brisanje korisnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564419"
---
# <a name="delete-tenant"></a>Brisanje korisnika

Da biste izbrisali Azure AD, provjerite sljedeće:
- Vi ste globalni administrator u direktoriju.
- Niste prijavljeni pomoću računa koji sadrži zadani direktorij, kao što je contoso.onmicrosoft.com u potpisu, kao što je admin@contoso.onmicrosoft.com.
- Prije brisanja uklonite sve aktivne aplikacije u direktoriju. Da biste uklonili aktivne aplikacije, dođite do registracija aplikacija i uklonite postojeće aplikacije.
- Ne postoje aktivne pretplate za bilo koji Microsoftov internetski servis, kao što su Microsoft Azure, Office 365 ili Azure AD Premium pridruženi direktoriju. Prenesite pretplate ili ubrzajte otkazivanje aktivnih pretplata putem podrške za Azure i naplate. Dodatne informacije o otkazu pretplate na Office 365 i Azure. Upute za povezivanje ili dodavanje postojeće pretplate na klijenta potražite u članku [pridruživanje ili dodavanje pretplate Azure u klijenta za Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Nema aktivne licence. Da biste uklonili licence, pročitajte članak [Kako ukloniti pretplatu da biste uklonili licencu](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Nema drugih aktivnih korisnika u imeniku osim sebe kao globalnog administratora prilikom pokušaja brisanja oglasa Azure. Uklonite sve druge aktivne korisnike, a sve ovisnosti o prilagođenom nazivu domene u zakupcu moraju biti uklonjene, kao što su korisnici koji su stvoreni uz admin@contoso.com.

Detaljne upute za:
- Brisanje "Azure Active Directory" ili "pretplata" potražite u članku [Brisanje servisa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Uklanjanje aplikacija u direktoriju potražite u članku [Uklanjanje aplikacija](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
