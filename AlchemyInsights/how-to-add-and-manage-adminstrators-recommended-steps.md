---
title: Dodavanje i upravljanje administratorima – preporučeni koraci
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676976"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>Dodavanje i upravljanje administratorima – preporučeni koraci

**Uređivanje administratora pretplate ili Suadministratora**

- Administrator računa može uređivati obje uloge dok administrator pretplate može promijeniti samo suadministratore na [portalu Azure](https://ms.portal.azure.com/#home).
- [Dodavanje ili promjena administratora pretplate na Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Ažuriranje administratora pretplate ili Co-Administrator za interne (emitiranja) pretplate**

Administrator servisa ili Suadministrator mogu samostalno služiti ovu akciju pomoću sljedećih koraka:

1. Prijavite se na [portal Azure](https://ms.portal.azure.com/#home) , a zatim kliknite **Upravljanje troškovima + naplata** u lijevoj oštrici.
2. Kliknite stavku na retku s pretplatom. Time ćete otvoriti pregled pretplate.
3. Na kartici **Pretplata** kliknite **Svojstva**. 
4. Kliknite gumb **administrator servisa** .
5. Unesite poruku e-pošte korisnika kojeg želite postaviti kao administratora servisa, a zatim kliknite **u redu**.

**Dodavanje/promjena/uklanjanje Suadministratora**

1. Prijavite se na [portal Azure](https://ms.portal.azure.com/#home) kao administrator servisa.
2. Otvorite [pretplate](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) , a zatim odaberite pretplatu. (Suadministratori se mogu dodijeliti samo u opsegu pretplate).
3. Pomaknite se do **kontrole Access (iam)**  >  **Classic administratori**  >  **dodatku** Dodaj  >  **suadministrator** da biste otvorili okno **Dodavanje suadministratora** (ako je mogućnost Dodaj suadministrator onemogućena, označava da nemate dozvole).
4. Odaberite korisnika kojeg želite dodati, a zatim kliknite **Dodaj**.

**uči više:**
- [Dodavanje Suadministratora](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Uklanjanje suadministratora](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Promjena administratora servisa](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Prikaz administratora računa](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Upravljanje pristupom pomoću portala RBAC i Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Dodavanje/brisanje korisnika pomoću servisa Azure Active Directory (AD)**

Možete dodati nove korisnike ili izbrisati postojeće korisnike iz tvrtke ili ustanove za Azure Active Directory (Azure AD):

1. Da biste dodali novog korisnika, prijavite se na [portal Azure](https://ms.portal.azure.com/#home) kao korisnik-administrator za tvrtku ili ustanovu.
2. Odaberite **Azure Active Directory**, odaberite **korisnici** , a zatim kliknite **novi korisnik**.
3. Na stranici **korisnika** unesite potrebne podatke. Kliknite **Stvori**. Korisnik se stvara i dodaje u zakupac Azure AD.

Dodatne **informacije**:

- [Dodavanje novog korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Brisanje korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Dodavanje i ažuriranje korisničkih podataka o profilu pomoću servisa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Preporučeni dokumenti**

- [Što je kontrola pristupa utemeljenih na ulogama (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Razumijevanje raznih uloga u servisu Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Dozvole za administratorsku ulogu u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Udžbenik: dodijelite pristup korisniku pomoću RBAC-a i portala Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Otklanjanje poteškoća s RBAC-om u servisu Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organiziranje resursa pomoću grupa za upravljanje Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Kako zatražiti kopiju Azure fakture putem e-pošte](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Dodavanje, ažuriranje ili uklanjanje kreditne ili debitne kartice iz servisa Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Upravljanje pretplatom (ponovno aktiviranje/otkazivanje/prebacivanje)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



